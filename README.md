# KNN Analysis based on TV Commercial Detection dataset

<!--
*** Thanks for checking out my groups text lab. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
-->


### Built With

* [RStudio Cloud](https://rstudio.cloud/)



<!-- GETTING STARTED -->
## Topic
For our Lab we did a KNN analysis of TV commercial data to classify when something is a commercial and when it is not. 

We started by determining the split between commercial and non-commercial data, and then we calculated the base rate, assuming that 1 is the commercial label and -1 is the non-commercial label. 

Following that initial step, we cleaned the data, removing columns that weren't relevant and that had greater than an absolute value of 0.7 in terms of variance to other features. 

We then generated a 80-20 split of training and testing data given our data set, and used the k-Nearest Neighbor to classify commercials in the testing data set. 

Using a k=3, we got that the:
* Accuracy is 76.76%
* Sensitivity is 86.73%
* Specificity is 59% 

A main goal of the lab was to help make more convincing commercials that hold audiences attention- making the company's commercials seem more like actual TV shows. 

We then ran the model with different odd numbers of k (between 1 to 21) using the KNN algorithm, and got that the most accurate and sensitive models were at k=7 and k=17. 

As mentioned before, our results were that the k=3 method had an accuracy of 76.76%, and a sensitivity of 86.73%. The k=7 (optimal) method on the other hand had an accuracy of 77.87% and a sensitivity of 89.26% (our base rate was about 63.9% accurate, which is a marked improvement).

Since our goal is to make commercials that are more like TV shows, it would be beneficial to observe when a commercial is classified as a false negative- basically when a TV clip is said not to be a commercial when it actually is (as explained before- this would be achieved by lowering the specificity value). A k=7 (optimal approach) compared to a k=3 results in a specificity reduction from 59% to about 57%. This is only a 2% reduction, so a greater magnitude of reduction is what we should be aiming for in our next analysis. 

So next time it will be better to focus solely on reducing the specificity value. This is probably the most relevant metric for creating the most convincing commercials that are perceived as non-commercials. 

Overall, we achieved the general goal of lowering the specificity using a k=7 model. 

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- CONTACT -->
## Contact

Sai Rajuladevi: https://www.linkedin.com/in/sai-rajuladevi/

Project Link: [https://github.com/sr9dc/DS_KNN_Lab_Group_6](https://github.com/your_username/repo_name)






