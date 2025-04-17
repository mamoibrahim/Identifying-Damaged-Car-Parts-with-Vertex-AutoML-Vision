# Identifying-Damaged-Car-Parts-with-Vertex-AutoML-Vision



# Step 1: uploading the training images to Cloud storage 

## 1.1 creating cloud storage bucket : 

```
export PROJECT_ID=$DEVSHELL_PROJECT_ID
export BUCKET=$PROJECT_ID
```

```
gsutil mb -p $PROJECT_ID \
 -c standard    \
 -l us-central1 \
 gs://${BUCKET}
```

## 1.2 uploading car images to out cloud storage bucket 

```
gsutil -m cp -r gs://car_damage_lab_images/* gs://${BUCKET}
```

# step 2: creating a dataset in VertexAI 


![image](https://github.com/user-attachments/assets/ff1db7de-5504-4dd0-8b2b-6ecfe4022bb2)



# step 3 : Connecting the dataset to the training images 

## (create a CSV file where each row contains a URL to a training image and the associated label for that image.)

![image](https://github.com/user-attachments/assets/07deb8f2-0292-4dc1-863d-22c715246fe4)


![image](https://github.com/user-attachments/assets/e0c37b24-00d2-47d6-acd6-8381ca97b32b)


# Training The Model

![image](https://github.com/user-attachments/assets/0112d493-4586-4a82-859d-861246e105de)


![image](https://github.com/user-attachments/assets/d12050ce-f91b-4954-982b-c5972c802a87)


