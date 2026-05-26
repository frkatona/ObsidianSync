### home
- applications
- reschedule mtnittany for end of month
- email HR
	- email Pennie
	- find out what to get and when for applying
	- ask what the premiums and out-of-pockets would be
	- ask Energy if they are in-network with Pennie
- reply 
	- Tim
	- Zack 
- live transcription app really useful...try to dockerize so I don't have to hunt it down each time and can share it easily
### work
- purchase Budget DN100CF laser air-free (vacuum + flow) chamber
	- $720 - cube ([ebay](https://www.ebay.com/itm/336467314008?chn=ps&google_free_listing_action=view_item))
	- $1200 - door, windowless ([Kurt J Lesker](https://www.lesker.com/flanges/fast-entry-access-load-lock-doors/part/ds-ll0600))
	- $450 - fused silica window ([ebay](https://www.ebay.com/itm/146888980432?chn=ps&google_free_listing_action=view_item))
	- $400 - swagelok adapter wall (1/4", gold) ([ebay](https://www.ebay.com/itm/404271163841))
		- $300 swagelok needle valve (1/4") ([Ideal](https://www.idealvac.com/en-us/Swagelok-Integral-Bonnet-Needle-Valve-14-in-Male-to-Female-NPT-6000-psig-009Cv-316-SS-PN:-SS-20KM4-F4/pp/P1011128))
		- $ ? - pump port (CF -> KF adapter)
		- $ ? - gas inlet (CF feedthrough)
		- $ ? - gas outlet/throttle
		- $ ? - gauge
	- remaining walls
		- {SOLD} $250 angled glass viewport ([ebay](https://www.ebay.com/itm/277469853023?_skw=6%22+flange+conflat+cf+door&itmmeta=01KP63371PCA1CM8V9N1KGZJSH&hash=item409a7df55f:g:hvQAAeSwyj9pAB4u&itmprp=enc%3AAQALAAABAGfYFPkwiKCW4ZNSs2u11xDtJgtjTldWxczS9yiMa4DooYqSBoyr5fX8gYFDInWnU7RSkYghTuYCDG2nXnlbCEwXWRk0rpn13FcOGxrrtO23hp0t6vAzUWN38U8xCScSrzKAPJnz119YpT0ZWR1qOxivB0leWhofSQ%2B2ieqN%2B%2FdUbqPTk60Lgf0AEpJSxdg01KLC0FTbad4qmlpvgm0Ybwh8AskRBUh8RPs1co%2BBQaKNIZqEqGqpNJrbsnnswM0Os1FU%2Bmq8oGnhX2DksJi%2BvM6%2BMLFAKBzMXidmuuym8OI9GYFv4Dz8uXRDkJn1eF%2Bj5Di7x3dv%2B005v%2FyBhlyLmQY%3D%7Ctkp%3ABk9SR5bxjMOxZw))
		- {SOLD} $50 glass viewport, cracked ([ebay](https://www.ebay.com/itm/366124886925?_trkparms=itmf%3D1%26aid%3D111001%26rkt%3D5%26algo%3DREC.SEED%26asc%3D20160811114145%26mech%3D2%26algv%3D%26pmt%3D0%26amclksrc%3DITM%26sid%3DAQALAAAAECEI3Cp75nyWeo%2Be%2FZqhp2U%3D%26itm%3D366124886925%26noa%3D1%26ao%3D1%26rk%3D7%26pid%3D100667%26b%3D1%26mehot%3Dnone%26lsid%3D0%26meid%3D932164247dcc41e0bb2c0bd3ebb2fa60%26pg%3D2334524&_trksid=p2334524.c100667.m2042))
		- $100 blank ([ebay](https://www.ebay.com/itm/298064350091?_skw=6%22+flange+conflat+cf+door&itmmeta=01KP63371R4YNGP0YEPW9N0K34&hash=item4566050b8b:g:HvMAAeSwovppno~R&itmprp=enc%3AAQALAAAA8GfYFPkwiKCW4ZNSs2u11xCmqJbuubo6XfzQJVj0U%2FvCg0YW4xkxIwdenUj8hC4cvBJ3X2%2FQuXvsf4rl%2FldSerMGoGzOU6%2FofWCGyonuCCCoqNm3ZSV3mgaim2l5z4OLSaWlbYhJSuarf%2FsMvsO7GPW2cqnbHzLTQG7o71bAfuQvQQ2XuU%2BoTqeBCrWIuQ6ZY3QINQuuxVrtJtRDSNKhdcwE2IYYpL8zsyNcPJl8UpHCmIbfyTbP7UjkMdgRVYGHTGSLl%2BZo7qHvd8ZD9DGVUiSlDVoEyO5aVpJXECJJy%2B6AQaIOvX4huyCXBazTf5IOQQ%3D%3D%7Ctkp%3ABk9SR5zxjMOxZw))
	- current total: ~$2500
- also purchase UV mirrorsflow chamber components
- Ben's project dockerization notes
	- just want an online fitting app?  does marimo not support these packages out of the box?  is there something that can't be pyodide'd?
		- otherwise, why not pyodide + github pages?
		- also, creating the dockerfile and using docker desktop + local web app is pretty straightforward as well
- meeting
	- lab jobs slide
	- read kristen's stats part to criticize
	- get a mockup of docker for Ben (static, offline docker desktop, and online container)

### subgroup
- Maybe new samples from Ben Stovall and AC this week
	- Rob on Ben about paper
	- next thin sample, do a million low power takes to deliver more total exposure, but at a rate that cannot increase temperature meaningfully
	- I should ask Tainara and AC if they can meet after Wednesday to get our expectations in order (when are the samples arriving, what is the time (and atmosphere) sensitivity, what tests need performed on them, how much sample needs allocated to which prep or analysis, when can I get them to Tainara and when can Tainara get to them, etc.)
- Ben Docker
	- blender
		- basic version success
		- profilometer progress
	- fitter
		- can do in a static site...what is it that you wanted?
		- libraries may expand image beyond ~500 MB limits for Google Cloud 'free tier'...are you will to pay a few bucks if something exceeds the guardrails?
- Tian-chi
	- scaring her over Marangoni flow
	- title of first paper something like "controlling topology in submerged PDMS coating cure through photothermal treatment"
		- my thought is that a baseline understand of all the most likely relevant chemical/physical phenomenon will be necessary or else the other ideas seem meaningless
		- also, 'marangoni flow' is strange to invoke as a rationale for defects and deformed/irregular textures since it is the reason for the regular textures
		- how to lean into the chemistry?
	- mechanism inventory
		- gel-front freezing
			- heating lowers viscosity initially, causing flow, then increases rapidly as crosslinking proceeds (freezing flow mid-motion)
			- test by allowing some amount of pre-cure
			- also applicable in-air (maybe future experiments should expand on in-air experiments to establish a better baseline)
		- other in-air: watching the bubbles for at slow-mo, changing up the de-gas parameter

Ben: "can you get the exact same with the parameters and expectations, then future work is what you could do to find what is actually different when you see it's different"

### Kaya/Bryan/Josh Docker explanation terminology
- https://docs.kernel.org/admin-guide/cgroup-v1/cgroups.html
- namespaces
- https://en.wikipedia.org/wiki/User_space_and_kernel_space
- https://blogs.oracle.com/linux/userspace-vs-kernelspace-understanding-the-divide