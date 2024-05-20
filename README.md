# XSS in CMSimple 5.15 (Settings -> Language)
**Software link:** CMSimple 5.15 [https://www.cmsimple.org/en/?Downloads___CMSimple]

**@author:** Antonio Díaz.

**Description:** Cross-site scripting (XSS) vulnerability in the Language section of the Settings menu of CMSimple 5.15 allow attackers to execute arbitrary web scripts or HTML via a crafted payload injected into multiple parameters.

**CVE:** CVE-2024-32344, CVE-2024-32345, CVE-2024-33423 y CVE-2024-33424.

## PoC
### Edit parameter (Action) (CVE-2024-32344)
1. Enter to Language section of the Settings menu:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/6036e7d4-899f-4dc4-9aa6-a60c859718b2)

2. Set the payload in 'Edit' parameter of the Action section:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/9d69b954-073a-49d3-a1fa-daaf07bc7376)

3. Click on the Save button:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/38e7ba88-b9cd-4ba7-a83c-23bfd886cb77)

4. Result:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/5fe39eee-c246-4aa8-abed-7bf7ea51f9fa)

### Configuration parameter (Adminmenu) (CVE-2024-32345)
1. Enter to Language section of the Settings menu:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/6036e7d4-899f-4dc4-9aa6-a60c859718b2)

2. Set the payload in 'Configuration' parameter of the Adminmenu section:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/5301952b-c67b-4815-9f08-750f8efa0695)

3. Click on the Save button:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/38e7ba88-b9cd-4ba7-a83c-23bfd886cb77)

4. Result:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/8e54abd2-cd96-429e-8160-6f1ef4c07953)

### Downloads parameter (Adminmenu) (CVE-2024-33424)
1. Enter to Language section of the Settings menu:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/6036e7d4-899f-4dc4-9aa6-a60c859718b2)

2. Set the payload in 'Downloads' parameter of the Adminmenu section:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/26841937-3e3e-4a07-be83-094466c111e9)

3. Click on the Save button:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/38e7ba88-b9cd-4ba7-a83c-23bfd886cb77)

4. Result:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/bef1bb69-1c1c-4af3-ae4b-0fe60f736bfa)


### Logout parameter (Adminmenu) (CVE-2024-33423)
1. Enter to Language section of the Settings menu:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/6036e7d4-899f-4dc4-9aa6-a60c859718b2)

2. Set the payload in 'Logout' parameter of the Adminmenu section:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/edf00cec-85f0-4a33-805a-b7c763db662a)

3. Click on the Save button:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/38e7ba88-b9cd-4ba7-a83c-23bfd886cb77)

4. Result:

![image](https://github.com/adiapera/xss_language_cmsimple_5.15/assets/165512291/26b30f0e-b194-47d1-9cff-0aa906259243)

### Note:
More parameters in the Settings section are vulnerable to XSS attacks.








