title: A New Measure for Analyzing Personal Networks
date: 2015-01-28 03:11:01
tags: [paper, facebook]
---
This is from [**Center of Attention: How Facebook Users Allocate Attention across Friends**](http://www.aaai.org/ocs/index.php/ICWSM/ICWSM11/paper/download/2899/3259). 

#### Notations
* $n$ individuals, $m\_j$ is the number of messages sent by person $i$ to $j$.  
* fraction of $i$'s attention devoting to $j$. 
$$a\_j=\frac{m\_j}{m}$$
* $TopK$ means top $K$ contacts with largest $a\_j$. 
{% math-block %}
f_k=\sum_{j \in TopK} a_j 
{% endmath-block%}

#### Knowledges
* Modalities
	* Communication
		* Messages
		* Comments
		* Wall Posts
	* Viewing
		* Profile Views
		* Photo Views

#### Results
* Distribution of Modalities ![](http://7u2qpd.com1.z0.glb.clouddn.com/5f893d05053b0ad42c0676ca8335c43df5b845ea-a109efd09ebdb0e9c90c6f5db41a67cc3a8e6ff9.png)
* Fraction $a\_k$ as a function of $k$ ![](http://7u2qpd.com1.z0.glb.clouddn.com/a9372c6e37090d828f57463ef6b9209795f5c16e-8964e49195fe30a09d118f2f3fabd73e858145af.png)
	* filter out the outliers (who do not significantly use each modality)
* Average fraction of attention devoted to top 15 contacts ![](http://7u2qpd.com1.z0.glb.clouddn.com/695f6e986ceef428d37398ab221a33e77c835983-18047bbafef6d1d5d82bb0097acfa8df3d8dadb9.png)
* Average fraction of messages sent to top 15 contacts as a function of network size and activity ![](http://7u2qpd.com1.z0.glb.clouddn.com/7c948ec680b96f0ddf3cdda904769cd84e89ca73-1ce7cfb320803bc4fae270f3f949603fbeccfe6c.png)
	* larger network leads to smaller $f\_{15}$ while more activity leads to larger $f\_{15}$
* $f\_{15}$ as a function of age ![](http://7u2qpd.com1.z0.glb.clouddn.com/a941e63a009b05c100cda735895c7d9cf2e864ed-c76c75dab89447898cde0a2b2399982b832d84e1.png)
* Distribution of attention given to top 5 friends for femailes and males ![](http://7u2qpd.com1.z0.glb.clouddn.com/00fc4dc94a5b2085a8b13735321306a83f4b2123-6765a3ac18a900cd646876ea1822eaadf3991486.png)
	* total activity and number of contacts vary significantly with age and gender
* $f\_5$, fixing genders 
	* messages ![](http://7u2qpd.com1.z0.glb.clouddn.com/2bec9c535c5de490df32dcf28e4d155cab70b9e8-b386af9c2a9c54097fc1ffa2e5f2c71855f51f7b.png)
	* profile views ![](http://7u2qpd.com1.z0.glb.clouddn.com/ba9aa40d06c58dab0ffbb93ea1764677cbaf3a71-abfc217c1506533f90a4ced9b3b4a23e490c46b7.png)
