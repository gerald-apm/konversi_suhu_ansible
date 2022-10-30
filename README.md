# Program konversi suhu menggunakan Ansible

Anda kira ansible hanya untuk automate infra saja? anda salah besar wkwkwk. Ansible bisa dibuat untuk apapun termasuk implementasi coding sederhana hehe.

## Sample output

```
Masukkan satuan suhu [celcius|fahrenheit|reamur|kelvin] (celcius):
Masukkan nilai suhu dalam satuan derajat/degree (100):

PLAY [Konversi suhu menggunakan ansible] ***********************************************************

TASK [Konversi suhu ke satuan lainnya] *************************************************************

TASK [convert_temperature : Konversi suhu celcius ke fahrenheit, reamur, dan kelvin] ***************
ok: [localhost]

TASK [convert_temperature : Konversi suhu fahrenheit ke celcius, reamur, dan kelvin] ***************
skipping: [localhost]

TASK [convert_temperature : Konversi suhu reamur ke celcius, fahrenheit, dan kelvin] ***************
skipping: [localhost]

TASK [convert_temperature : Konversi suhu kelvin ke celcius, reamur, dan fahrenheit] ***************
skipping: [localhost]

TASK [convert_temperature : Formatting hasil konversi °] *******************************************
ok: [localhost]

TASK [Keluarkan hasil konversi] ********************************************************************
ok: [localhost] => {
    "hasil_konversi": {
        "celcius": "100.00°C",
        "fahrenheit": "212.00°F",
        "kelvin": "373.15°K",
        "reamur": "80.00°R"
    }
}

PLAY RECAP *****************************************************************************************
localhost                  : ok=3    changed=0    unreachable=0    failed=0    skipped=3    rescued=0    ignored=0
```
