# GS1_oneM2M_MMG
------------------------------------

## To start GS1_oneM2M_MMG 

1. Run MQTT for EPCIS 
2. Run EPCIS with MQTT Enabled 
3. Run GS1_oneM2M_MMG 

once the GS1_oneM2M_MMG  is running, configure it using POST as follows

|  // |       |
| ------------- | ------------- |
| POST   | http://[IP]:[PORT]/post_gs1 |
| Header    | [{"key":"Accept","value":"application/onem2m-resource+xml","description":""},{"key":"Content-Type","value":"application/json","description":""},{"key":"X-M2M-RI","value":"1234534","description":""},{"key":"X-M2M-Origin","value":"SOrigin","description":""}]   |
| Body   | { "epcis_ip":"[IP]",  "epcis_port":"[PORT]",  "oneM2M_ip":"[IP]",  "oneM2M_port":"[PORT]",  "oneM2M_mqtt_port":"[PORT]", "epcis_ip_mqtt":"[IP]",  "epcis_port_mqtt" : "[PORT]" }   |


### Additional Notes 
... Use Spring boot
... Sample postman collection is provided for test under the example directory

## License
[Apache License 2.0](https://github.com/yalewkidane/GS1_oneM2M_MMG/blob/master/LICENSE)
