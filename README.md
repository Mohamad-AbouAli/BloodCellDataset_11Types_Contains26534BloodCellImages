# Blood Cell Revolution: Unveiling 11 Distinct Types with ‘Naturalize’ Augmentation
This paper introduces the **‘Naturalize’** technique, improving the classification of 11 blood cell types through deep learning and image processing. This approach enhances diagnostic accuracy in hematology. For more details, check the [full paper](https://www.mdpi.com/1999-4893/16/12/562).

## Transition from 8-Class PBC to 11-Class PBC
This transition expands the classification of published peripheral blood cells (PBC) dataset from 8 to 11 distinct types, improving the granularity and accuracy of cell identification.

![Transition to 11-Class PBC](https://www.mdpi.com/algorithms/algorithms-16-00562/article_deploy/html/images/algorithms-16-00562-g003-550.jpg)


## PBC Images Containing More Than One Class
This step demonstrates peripheral blood cell (PBC) images that contain multiple classes. The image showcases the complexity of classifying different blood cell types in a single image.

![PBC Images](https://www.mdpi.com/algorithms/algorithms-16-00562/article_deploy/html/images/algorithms-16-00562-g004-550.jpg)

## Algorithm: Naturalize Algorithm

1. **Imports and Paths**  
   Import required libraries and define file paths.
   
2. **Load SAM_model and PBC Dataset**  
   - Mount Google Drive  
   - Load peripheral blood smear images from the PBC dataset  
   - Load SAM model

3. **Segment PBC Dataset Using SAM**  
   - Segment images into "RBCs, WBCs, PLTs"  
   - Save segmented images to Google Drive

4. **Collision Function**  
   - Function to check for image collisions

5. **Composite Image Creation**  
   - For each image, load background, add WBCs, RBCs, and avoid collisions  
   - Save the composite image

## Step 1: Segmentation
The first step of the **Naturalize** algorithm involves segmenting peripheral blood smear images into distinct cell types: RBCs, WBCs, and PLTs. This is done using the Segment Anything Model (SAM) model developed by Meta AI.

![Segmentation](https://www.mdpi.com/algorithms/algorithms-16-00562/article_deploy/html/images/algorithms-16-00562-g005-550.jpg)

## Step 2: Composite Image Generation
In the second step, composite images are generated by adding WBCs and RBCs while avoiding collisions.

![Composite Image](https://www.mdpi.com/algorithms/algorithms-16-00562/article_deploy/html/images/algorithms-16-00562-g006-550.jpg)

## Score-CAM for Fine-Tuned DenseNet-169
The Score-CAM method is applied to visualize the areas of an image that contribute most to the model's decision. In this case, the method is used with a fine-tuned DenseNet-169 model to understand its predictions better.

![Score-CAM](https://www.mdpi.com/algorithms/algorithms-16-00562/article_deploy/html/images/algorithms-16-00562-g011-550.jpg)


## 📚 References

### MDPI and ACS Style  
Abou Ali, M.; Dornaika, F.; Arganda-Carreras, I. *Blood Cell Revolution: Unveiling 11 Distinct Types with ‘Naturalize’ Augmentation*. **Algorithms** 2023, *16*, 562. [https://doi.org/10.3390/a16120562](https://doi.org/10.3390/a16120562)

### AMA Style  
Abou Ali M, Dornaika F, Arganda-Carreras I. *Blood Cell Revolution: Unveiling 11 Distinct Types with ‘Naturalize’ Augmentation*. **Algorithms**. 2023; 16(12):562. [https://doi.org/10.3390/a16120562](https://doi.org/10.3390/a16120562)

### Chicago/Turabian Style  
Abou Ali, Mohamad, Fadi Dornaika, and Ignacio Arganda-Carreras. 2023. "*Blood Cell Revolution: Unveiling 11 Distinct Types with ‘Naturalize’ Augmentation*." **Algorithms** 16, no. 12: 562. [https://doi.org/10.3390/a16120562](https://doi.org/10.3390/a16120562)

### APA Style  
Abou Ali, M., Dornaika, F., & Arganda-Carreras, I. (2023). *Blood Cell Revolution: Unveiling 11 Distinct Types with ‘Naturalize’ Augmentation*. **Algorithms, 16**(12), 562. [https://doi.org/10.3390/a16120562](https://doi.org/10.3390/a16120562)


```bibtex

@Article{a16120562,
AUTHOR = {Abou Ali, Mohamad and Dornaika, Fadi and Arganda-Carreras, Ignacio},
TITLE = {Blood Cell Revolution: Unveiling 11 Distinct Types with ‘Naturalize’ Augmentation},
JOURNAL = {Algorithms},
VOLUME = {16},
YEAR = {2023},
NUMBER = {12},
ARTICLE-NUMBER = {562},
URL = {https://www.mdpi.com/1999-4893/16/12/562},
ISSN = {1999-4893},
DOI = {10.3390/a16120562}
}
