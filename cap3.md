# Capstone 3 project ideas

1. continue development of campsite prediction with some of these ideas

* try transfer learning models
* Clean training data
* more data, more diversity
* pull random sat images as "not campsite"
* determine the actual campsite coordinates within the image (patch detect?)
* Try sobel transformation
* Include additional binary columns such as “bathrooms” etc
* Utilize NLP topics to aid image classification
* Multiclassification
* Train with additional sat images
* Implement class weights
* NLP with higher level tokens than words
* Examine F1 scores
* More dropouts in model

2. transcribed farmer reported issues in India to be combined with other modeling approaches to detect new issues based on what they are talking about. 5 million records for the period 2009-2020. 

The data looks like this:

|   Season | Sector       | Category   | Crop                                              | QueryType        | QueryText                                                                     |   KccAns | StateName     | DistrictName   | BlockName     | CreatedOn               |
|---------:|:-------------|:-----------|:--------------------------------------------------|:-----------------|:------------------------------------------------------------------------------|---------:|:--------------|:---------------|:--------------|:------------------------|
|      nan | AGRICULTURE  | Cereals    | Paddy (Dhan)                                      | Weather          | Information about weather forecast of Distrect-Etah in Block- Shitalpur.....? |      nan | UTTAR PRADESH | ETAH           | SHITALPUR     | 2019-10-01T06:13:39.82  |
|      nan | HORTICULTURE | Vegetables | Cabbage                                           | Plant Protection | Plant protection measures insect control in cabbage crop ?                    |      nan | UTTAR PRADESH | ETAH           | ALIGANJ       | 2019-10-01T06:14:00.29  |
|      nan | AGRICULTURE  | Others     | Others                                            | Weather          | Information about weather forecast of Block jalesar  in District etah ?       |      nan | UTTAR PRADESH | ETAH           | AWAGARH       | 2019-10-01T06:43:00.063 |
|      nan | AGRICULTURE  | Cereals    | Paddy (Dhan)                                      | Plant Protection | dhan me brawon plant hopper laga hai ?                                        |      nan | UTTAR PRADESH | ETAH           | AWAGARH       | 2019-10-01T06:46:36.063 |
|      nan | AGRICULTURE  | Others     | Others                                            | Weather          | Information about weather forecast of Block   Aliganj  in District  Etah   ?  |      nan | UTTAR PRADESH | ETAH           | ALIGANJ       | 2019-10-01T06:47:58.947 |
|      nan | AGRICULTURE  | Others     | Others                                            | Weather          | Please give me information for weather to district -etah..?                   |      nan | UTTAR PRADESH | ETAH           | ALIGANJ       | 2019-10-01T06:50:10.13  |
|      nan | AGRICULTURE  | Others     | Others                                            | Weather          | Information about weather forecast of Block Jaithra in District Etah....?     |      nan | UTTAR PRADESH | ETAH           | JAITHARA      | 2019-10-01T06:54:03.663 |
|      nan | AGRICULTURE  | Others     | Others                                            | Weather          | TELL ME ABOUT WEATHER INFORMATION ?                                           |      nan | UTTAR PRADESH | ETAH           | GANJ DUNDWARA | 2019-10-01T07:35:07.143 |
|      nan | AGRICULTURE  | Others     | 0                                                 | Weather          | Information about weather forecast of Block soron in District etah?           |      nan | UTTAR PRADESH | ETAH           | SORON         | 2019-10-01T07:35:10.047 |
|      nan | AGRICULTURE  | Millets    | Pearl Millet (Bajra/Bulrush Millet/Spiked Millet) | Plant Protection | Control of stem borer in pearl millet crop...?                                |      nan | UTTAR PRADESH | ETAH           | SORON         | 2019-10-01T07:38:04.237 |

3. plant disease image detection
https://www.kaggle.com/c/plant-pathology-2020-fgvc7/data

