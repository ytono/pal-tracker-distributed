```shell script
REGISTRATION_APP_URL=registration-pal-yt.apps.evans.pal.pivotal.io
BACKLOG_APP_URL=backlog-pal-yt.apps.evans.pal.pivotal.io
ALLOCATIONS_APP_URL=allocations-pal-yt.apps.evans.pal.pivotal.io
TIMESHEETS_APP_URL=timesheets-pal-yt.apps.evans.pal.pivotal.io
```

cd ~/workspace/assignment-submission
./gradlew cloudNativeDeveloperDistributedSystemDeployment \
    -PregistrationServerUrl=https://${REGISTRATION_APP_URL} \
    -PbacklogServerUrl=https://${BACKLOG_APP_URL} \
    -PallocationsServerUrl=https://${ALLOCATIONS_APP_URL} \
    -PtimesheetsServerUrl=https://${TIMESHEETS_APP_URL}