# hexo-githubåšå®¢æ­å»ºè¿‡ç¨‹
å‚è€ƒï¼šhttps://www.cnblogs.com/liuxianan/p/build-blog-website-by-hexo-github.html

### 1. å®‰è£…Node.js
### 2. å®‰è£…Git
### 3. å®‰è£…Hexo
	æ‰“å¼€cmdï¼Œæ‰§è¡Œnpm install hexo-cli -g
	ç­‰å¾…å®‰è£…å®Œæˆåï¼Œè¾“å…¥hexo -væ£€æŸ¥æ˜¯å¦å®‰è£…æˆåŠŸ
### 4. githubä¸Šæ–°å»ºåšå®¢åº“username.github.io
### 5. åˆå§‹åŒ–Hexo
	æ–°å»ºæ–‡ä»¶å¤¹ç”¨äºå­˜æ”¾hexoï¼Œæ‰§è¡Œhexo initï¼›
	åŠ è½½hexoåŸºç¡€htmlã€cssã€jsç­‰æ–‡ä»¶ï¼šhexo g
	æœ¬åœ°å¯åŠ¨ hexo sï¼ŒéªŒè¯æ˜¯å¦é…ç½®æˆåŠŸ
### 6. hexoä¸»é¢˜ï¼Œé…ç½®ä¿®æ”¹
	ï¼ˆ1ï¼‰å®‰è£…ä¸»é¢˜ï¼ˆhttps://hexo.io/themes/ï¼‰
	git clone https://github.com/iissnan/hexo-theme-next themes/next
	ï¼ˆ2ï¼‰å›åˆ°hexoæ ¹ç›®å½•ç”¨è®°äº‹æœ¬æ‰“å¼€_config.xmlæ–‡ä»¶ï¼Œä¿®æ”¹landscape,æ”¹æˆ nextï¼›
	ï¼ˆ3ï¼‰ä¿®æ”¹_config.yml
		é…ç½®Siteå†…å®¹ï¼ŒDeploymentï¼ˆè¿œç¨‹ä»“åº“åœ°å€ï¼‰ï¼›
### 7. éƒ¨ç½²
	ï¼ˆ1ï¼‰å®‰è£…éƒ¨ç½²å·¥å…·
		npm install hexo-deployer-git -save
<<<<<<< HEAD
	£¨2£©³õÊ¼»¯±¾µØ²Ö¿âgit init
	£¨4£©·¢²¼hexoµ½github
		hexo clean && hexo g && hexo d
### 8. Ğ´²©¿Í
	£¨1£©¶¨Î»µ½hexo¸ùÄ¿Â¼£¬Ö´ĞĞ hexo new ¡°test¡±£¬»áÔÚ_postsÏÂÉú³ÉmdÎÄ¼ş£»
	£¨2£©ĞŞ¸ÄmdÎÄ¼ş
		ÍêÕû¸ñÊ½£º
		---
		title: postName #ÎÄÕÂÒ³ÃæÉÏµÄÏÔÊ¾Ãû³Æ£¬Ò»°ãÊÇÖĞÎÄ
		date: 2013-12-02 15:30:16 #ÎÄÕÂÉú³ÉÊ±¼ä£¬Ò»°ã²»¸Ä£¬µ±È»Ò²¿ÉÒÔÈÎÒâĞŞ¸Ä
		categories: Ä¬ÈÏ·ÖÀà #·ÖÀà
		tags: [tag1,tag2,tag3] #ÎÄÕÂ±êÇ©£¬¿É¿Õ£¬¶à±êÇ©ÇëÓÃ¸ñÊ½£¬×¢Òâ:ºóÃæÓĞ¸ö¿Õ¸ñ
		description: ¸½¼ÓÒ»¶ÎÎÄÕÂÕªÒª£¬×ÖÊı×îºÃÔÚ140×ÖÒÔÄÚ£¬»á³öÏÖÔÚmetaµÄdescriptionÀïÃæ
		---

		ÒÔÏÂÊÇÕıÎÄ
	£¨3£©²©ÎÄ²»ÏÔÊ¾È«²¿ÄÚÈİ
		ÊÇÔÚºÏÊÊµÄÎ»ÖÃ¼ÓÉÏ<!--more-->¼´¿É
		
=======
	ï¼ˆ2ï¼‰åˆå§‹åŒ–æœ¬åœ°ä»“åº“git init
	ï¼ˆ4ï¼‰å‘å¸ƒhexoåˆ°github
		hexo clean && hexo g && hexo d

		
		
>>>>>>> 01db3a425fd5d1e65daf323f7ad1d60de5c0bc18
