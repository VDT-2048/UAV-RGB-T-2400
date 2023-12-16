# UAV-RGB-T-2400
# Image Acquisition System
We use a professional UAV (DJI MAVIC 2 Enterprise Advanced) to capture the images, as shown in Fig. (a). The UAV has an infrared camera and a visible light camera. And the UAV can record video of the same scene simultaneously. The infrared camera has a resolution of 640-512 , and the visible camera has a resolution of 1920-1080.
# Image Acquisition Location
The UAV RGB-T 2400 dataset is mainly based on campus scenes. Various scenes are selected on campus to collect the images throughout the day. The main image acquisition scenes include parks, woods, roads, stadiums, near teaching buildings,
parking lots, restaurants, and other places. In Fig.(b), we detail the image acquisition location. In addition, to improve the object richness of the dataset, we also collect some images in the off-campus park, including some military and aerospace models.
# Dataset Construction Process
The specific construction process of the dataset is shown in Fig. (c). First, the UAV are used to capture videos of scenes containing specific objects in the same place at the same time. For this UAV, only the way of capturing video can ensure that the two modalities have space-time synchronization. Then, the video deframing algorithm is then used to deframe videos in visible light and thermal infrared modalities. Next, we select the image pairs with considerable differences from the image sequences as our dataset. Due to the different imaging principles of visible light and thermal infrared, the number of images after deframing visible light and thermal infrared videos with the same length is different. Therefore, the selection process needs to be carefully selected manually so that the images of the two modalities correspond exactly. However, we keep some of the time misaligned image pairs in our dataset to make the dataset close to the actual scene.

![Acquisition Location](https://github.com/VDT-2048/UAV-RGB-T-2400/assets/101933818/6dbd8c9a-06fd-4d50-b7e8-95983dbb261a)


# Download Dataset

The dataset is available at：https://pan.baidu.com/s/1dsQP-i1H7X1OGw0UxBjnEg?pwd=ifyh

# Challenging Scenes
In real life, UAVs are often used in various industries, and the working environment is complicated. To conform to the actual situation as much as possible, the UAV RGB-T 2400 dataset contains five categories of challenges and twenty-one
sub-categories, as shown in Fig. (a). The five main challenges include variable illumination, variable object, object blur, variable weather, and object occlusion. First, we collect images of different real-life illumination scenes, including illumination intensities and sources. There are several sub-categories of illumination challenges: low illumination (LI), extreme low illumination (ELI), street light exposure (SLE), UAV light exposure (ULE), shadow interference (SI), sunlight exposure (SE), and exposure interference (EI). The detection objects of UAVs vary, and the positions of objects in the image are also different. Therefore, the object challenges in our dataset mainly include the following five sub-categories: small salient object (SSO), multiple salient objects (MSO), center bias (CB), outof-view (OV), and scale variation (SV). In addition, in the process of UAV detection, the UAV may fly fast, or the object may move quickly, resulting in blurred images. So the object blur challenges mainly include the following two subcategories: fast object movement (FOM) and fast UAV movement (FVM). Weather changes are unavoidable during UAV detection, so we also collect some weather challenges: rain (R), snow (S), and fog (F). It’s worth noting that we simulate foggy days with artificial smoke. Finally, object occlusion is also one of the common challenges of UAV detection. Here we have collected four object occlusion challenges: tree occlusion (TO), plastic occlusion (PO), umbrella occlusion (UO), and glass occlusion (GO).
We conduct tests in these challenging scenes and conduct comparative experiments. 
The testing datasets divided by challenging scenes is available at: Test Data(challenge)

![Challenging Scenes](https://github.com/VDT-2048/UAV-RGB-T-2400/assets/101933818/eae6a763-6c47-4785-95d0-f52643bfd023)


# Saliency Maps of All Compared Methods
The saliency maps of all compared methods on the UAV RGB-T 2400 testing dataset are provided at: Saliency maps (Comparison experiment) https://pan.baidu.com/s/1dsQP-i1H7X1OGw0UxBjnEg?pwd=ifyh

The test results and comparative experimental results on these challenging scenes are provided at: saliency maps (Challenge comparison) https://pan.baidu.com/s/1dsQP-i1H7X1OGw0UxBjnEg?pwd=ifyh

# Evalution Toolbox
The evalution toolbox is provided by https://github.com/jiwei0921/Saliency-Evaluation-Toolbox
