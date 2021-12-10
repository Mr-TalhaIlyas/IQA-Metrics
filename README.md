# Measure-similarity-in-images

### Sample Image

![alt text](https://miro.medium.com/max/1400/1*GWmJfFwoPj2_M03Qyd8nxQ.png)
First install package

```
pip install sewar
```

Then import necessary packages.

```
from sewar.full_ref import mse, rmse, psnr, uqi, ssim, ergas, scc, rase, sam, msssim, vifp
```

Define/ Load images

```
org = cv2.imread()
blur = cv2.imread()

# get measurements

print("MSE: ", mse(blur,org))
print("RMSE: ", rmse(blur, org))
print("PSNR: ", psnr(blur, org))
print("SSIM: ", ssim(blur, org))
print("UQI: ", uqi(blur, org))
print("MSSSIM: ", msssim(blur, org))
print("ERGAS: ", ergas(blur, org))
print("SCC: ", scc(blur, org))
print("RASE: ", rase(blur, org))
print("SAM: ", sam(blur, org))
print("VIF: ", vifp(blur, org))
```
Scores from the similarity metrics for different types of noising methods

![alt text](https://miro.medium.com/max/700/1*NuN5Xm8tLzsbhT1fsmHkWg.png)

## Reference
[Measuring similarity in two images using Python @ TowardsDataSceince by Param Raval](https://towardsdatascience.com/measuring-similarity-in-two-images-using-python-b72233eb53c6)
