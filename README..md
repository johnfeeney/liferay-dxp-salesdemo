# First deploy the services using the script
```
./wedeploy.sh
```

# Steps required after deploying the services

```
we shell -s liferay -p liberty
cd /wedeploy-container/staticdata
cp -r * /opt/liferay/data/document_library
exit
we restart -s liferay -p salesdemo
```