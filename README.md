Using Keras model.fit_generator for training optimization

Purpose: Less GPU memory usage(<8Gb) and higher training accuracy 


Original project: NCHC scenario test "Task A:Visual-Speed Detection"
https://github.com/TW-NCHC/functionality-scenario-test-A-2018

Step1: Setup all environment and running well as upper NCHC URL link

Step2: Separated validation dataset. 
       Cut 1/10 *.pkl from /datasets to /datasets_val for validation

Ex.	/functionality-scenario-test-A-2018-master
		/weights	
		/datasets
			/nfbCCTV-N1-N-90.01-M	---->> cut 1/10 for validation
		/datasets_val			   
			/nfbCCTV-N1-N-90.01-M   <<---- paste
		/cctv_imgs
		train.py
		prepare.py
		feed.py

Step3: Run this new version of  "train.py -e 20 -l 0 -w "./weights"
