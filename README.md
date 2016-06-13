AutoCog is a tool to assess how well an Android application description reveal the security-concerned permission in semantics level. Based on our learning approach, the tool leverages large-scale of Android applications and descriptions to generate a Description-to-Permission Relatedness (DPR) Model (semantic patterns and permission with high correlation). 

We porvide the Web API:
----------------------------------------------------------------------------------------------------
You may retrieve the questionable permissions and the permissions described from each sentence by the API: http://garuda.cs.northwestern.edu:8888/?name=PACKAGENAME. Each operation might take seconds to minutes for the background analysis.

Example:
garuda.cs.northwestern.edu:8888/?name=com.ultimarom.launchnavigation


result:0
Questionable Permission:{u'com.ultimarom.launchnavigation': [u'RECEIVE_BOOT_COMPLETED', u'ACCESS_COARSE_LOCATION']}
Description and Permission:{u'com.ultimarom.launchnavigation': [[u'This app is NOT a navigation app', [u'ACCESS_FINE_LOCATION']], [u"If you're like me, you'll miss this icon", []], [u'This app puts it back', []], [u"See the developers' sites for those kinds of issues", []], [u'Google removed the Navigation icon for Maps with an update', []], [u'Any issues regarding location, Maps crashing or internet use are not anything to do with this app', []], [u'It simply opens Google Navigation in one click, rather than a few', []]]}

Result 0 indicates a successful invocation.

----------------------------------------------------------------------------------------------------
If you would like to cite our work:
@inproceedings{qu2014autocog,
  title={Autocog: Measuring the description-to-permission fidelity in android applications},
  author={Qu, Zhengyang and Rastogi, Vaibhav and Zhang, Xinyi and Chen, Yan and Zhu, Tiantian and Chen, Zhong},
  booktitle={Proceedings of the 2014 ACM SIGSAC Conference on Computer and Communications Security},
  pages={1354--1365},
  year={2014},
  organization={ACM}
}
