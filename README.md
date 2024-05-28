# dependencies-scanning
Notes from DevSecOps ch.5 Vulnerability Scanning Application Dependencies

To check dependencies for vulnerabilities -> Software Composition Analysis (SCA)
= checks public library databases (storing CVEs) for the latest secure version for the dependencies and recommends updating dependency to that version

Various tools for each language 
node -> npm audit
javascript -> retire.js

We can extend our pipeline script and python script to handle downloading/uploading or retire.js scan files into DefectDojo
<img width="565" alt="Capture d’écran 2024-05-28 à 21 22 30" src="https://github.com/JulienAvezou/dependencies-scanning/assets/62488871/6c4f09bf-7fb3-423f-a657-801dbe7a931b">
<img width="274" alt="Capture d’écran 2024-05-28 à 21 22 43" src="https://github.com/JulienAvezou/dependencies-scanning/assets/62488871/28702bcd-2aa4-4b1e-ad5f-964c3ceb342d">

<img width="443" alt="Capture d’écran 2024-05-28 à 21 32 38" src="https://github.com/JulienAvezou/dependencies-scanning/assets/62488871/96a6efe2-dfac-4658-b467-fc30186c464c">
<img width="1307" alt="Capture d’écran 2024-05-28 à 21 33 52" src="https://github.com/JulienAvezou/dependencies-scanning/assets/62488871/0fb2c445-1ee5-40f3-ae1f-3b65f2de61d5">

Updating major Library versions is not always straightforward as it can contain breaking changes so it is important to understand this on the development side
