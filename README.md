# galakto-token-diy
Creating a diy version of a galakto token


# hardware (token-specific)

There seem to be several different hardware revisions of galakto tokens with regards to the flash chip used. On the package there is a marking indicating the flash chip. e.g. TVORO1

# data structure


```bash
├── mcu_ota_4b71d.bin
├── mcu_ota_4b71d.bin.sig
├── System Volume Information
│   ├── IndexerVolumeGuid
│   ├── IndexVolumeGuid
│   │   ├── 00000.mp3
│   │   ├── 00000.mp3.hashes
│   │   ├── 00000.mp3.hashes.sig
│   │   ├── 00001.mp3
│   │   ├── 00001.mp3.hashes
│   │   ├── 00001.mp3.hashes.sig
│   │   ├── 00002.mp3
│   │   ├── 00002.mp3.hashes
│   │   ├── 00002.mp3.hashes.sig
│   │   ├── 00003.mp3
│   │   ├── 00003.mp3.hashes
│   │   ├── 00003.mp3.hashes.sig
│   │   ├── 00004.mp3
│   │   ├── 00004.mp3.hashes
│   │   ├── 00004.mp3.hashes.sig
│   │   ├── 00005.mp3
│   │   ├── 00005.mp3.hashes
│   │   ├── 00005.mp3.hashes.sig
│   │   ├── 00006.mp3
│   │   ├── 00006.mp3.hashes
│   │   ├── 00006.mp3.hashes.sig
│   │   ├── 00007.mp3
│   │   ├── 00007.mp3.hashes
│   │   ├── 00007.mp3.hashes.sig
│   │   ├── 00008.mp3
│   │   ├── 00008.mp3.hashes
│   │   ├── 00008.mp3.hashes.sig
│   │   ├── 00009.mp3
│   │   ├── 00009.mp3.hashes
│   │   ├── 00009.mp3.hashes.sig
│   │   ├── 00010.mp3
│   │   ├── 00010.mp3.hashes
│   │   ├── 00010.mp3.hashes.sig
│   │   ├── 00011.mp3
│   │   ├── 00011.mp3.hashes
│   │   ├── 00011.mp3.hashes.sig
│   │   ├── 00012.mp3
│   │   ├── 00012.mp3.hashes
│   │   ├── 00012.mp3.hashes.sig
│   │   ├── 00013.mp3
│   │   ├── 00013.mp3.hashes
│   │   ├── 00013.mp3.hashes.sig
│   │   ├── 00014.mp3
│   │   ├── 00014.mp3.hashes
│   │   ├── 00014.mp3.hashes.sig
│   │   ├── 00015.mp3
│   │   ├── 00015.mp3.hashes
│   │   ├── 00015.mp3.hashes.sig
│   │   ├── all-files.hashes
│   │   ├── all-files.hashes.sig
│   │   ├── check.txt
│   │   ├── settings.properties
│   │   ├── settings.properties.sig
│   │   └── signature.txt
│   └── WPSettings.dat
├── update_159e6.ufw
└── update_159e6.ufw.sig
```

# Security

If you combine all hases of the mp3 files, you get the following result:

```
3046022100ebbd8cd4da5628375fafef37e30b2787bd2181a1336ee2632645874261286123022100f5751c049161efbe73a6e13fb509e9b06a99e1a8c035f37cef6fdeece556e176
30440220208ab6988ee9cef4db7155e0854f4658880c3cfe368b685ab0c5e1b9d1dbf2ce022075690baa8c5594515fb725364abcdcefb4c575fcaa3d6a85c3ddb460899e685b
304402201e2cb78cc7dcdadacaceb6b839ba1f4374c8887626fbe147db1e3c4a4b5069ad02200b7436fa1b1723e1dc60b423ce195edc3a218d9d7ff6d06bc5a8dacfdd123f77
3045022100d37eada40687818e1e6cf66e5d0fda33c36425d0e7dca677986d9f6fb31d28940220773f9c6d4b17bdc7f44c3a4adefa4766b76f473dd933536fe8e5e2e6f134f97c
3045022100baf24a84a28295d1b1a7d5555c655529479fbc94ee584d79f29d317fdd71866402207f4c7d39d7c93d914b052fd3bf8fabcea8ff874d171365da398595ff5417f3a3
304502204a61104e72d660b42500a46b8fe83914f02aa5b893e6cb001ecc9829b971c37d022100b6fe0ea5a7f8843a36f86402b9963d05975ee08b5c6c18b4a21d73c5ea383b39
3046022100efb3c2e23655b349cbece03572f376d40ecf734211f6176aa791cf0644dbc1e50221009988d9f869839abe4e9dc672a5ee8fa22ccf21a5faa04654033b8d2c3c4cc9c7
304402200777325a21f09c63b9059617325cd186e84fc2883128127787c8418da57d4254022062cb274ea1637cafcc446aee530b254d9acbf09ed965a0d0ade8874ffc0f98b9
3045022054937d311f988515759dbf7ecf498f45045533088a0ae3d7ddac7a4602aca18b022100dd3c7145dc9f93ea55e84bef5a06b7603aa17ee1207b4e535e1feef17b51cfaf
3045022100ecdfb568d87a574aecf62c21f98f7d561c3cc6ccfd4ecbc11086a8af3245cacb022039a3377e27d201c201fff1df78603bbe7ec899c1f585404efb1ba6c01e8f7c36
3045022100a4493f698894f6b6765ed5c829f820100a5098accead5f2acdc0831c380eb62e02207a5a36569a091a99c60d072d07b3577a95013559b26c3d75590aae263c0b9b0e
3045022100c59528d2f43c4798c17a13204d3650a3290164257b8a9e507b6df02cf6b11dba022067fae738672f81fe791fbe446a4f52461a5d78275fdfcf06791fb203a90901ae
304502206180defb0c732719378f9682ef0711ca52ae796f87e77a66bdddbf400f79e671022100d8a55fd4daca708a6a0b5be372438e28cdf61ae34f80f18448d87a076f74a646
3046022100c5596d8dcf5e8a3cfab12c365c5040895390b1ddb46e39a0bf42a5500e2ad000022100cd2b2d0526976205769fe46703e5588c7b3353cb974c55c596424ecd1e919f6e
3045022100ba4f763ee18f6dfb8e0bd3683884cef6b40ecb0c56129ab9ee4e9ffb4a9b42b802200c84f7dbd8e37d2b90de631493b3067c9574c3846591890a2685a1829c6eee69
30440220247271e337eefd6dd0e443e4ce2ce2e3730fb84faab843256c82a70d211e4d0e02204f451b094d9f0e488a783be085dead2c85f390bf95833e77304ae75b15dcfcb4
```

The lines are all starting with 30 and then a value between 44 and 46 indicating the length of the signature. Then there is a 0220 or 0221. This happens in the mid of the signature again.
If there are two 0220 in the line, the value is 44, if there is at least one 0221 then its 45 and when there are two 0221 then the value is 46.
