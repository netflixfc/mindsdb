# MindsDB API Reference (เอกสารอ้างอิง API ของ MindsDB)

## Overview (ภาพรวม)
MindsDB is an open-source machine learning platform that allows you to develop models and make predictions directly from your database. The API provides endpoints for various tasks such as model training, prediction, and reporting.

## API Endpoints (จุดสิ้นสุด API)

### 1. Create Model (สร้างโมเดล)
- **Endpoint:** `/api/v1/models`
- **Method:** `POST`
- **Description:** Creates a new ML model based on the provided training data.

### 2. Train Model (ฝึกโมเดล)
- **Endpoint:** `/api/v1/models/{model_id}/train`
- **Method:** `POST`
- **Description:** Trains the specified model using the data you provide.

### 3. Make Prediction (สร้างการพยากรณ์)
- **Endpoint:** `/api/v1/predict`
- **Method:** `POST`
- **Description:** Sends data to the model and receives predictions.

### 4. Get Model Status (ตรวจสอบสถานะโมเดล)
- **Endpoint:** `/api/v1/models/{model_id}/status`
- **Method:** `GET`
- **Description:** Retrieves the training and prediction status of the specified model.

## Authentication (การพิสูจน์ตัวตน)
- All API requests require an API key. You can generate it from your MindsDB dashboard.

## Example Request (การร้องขอตัวอย่าง)
```json
{
  "data": {
    "column1": "value1",
    "column2": "value2"
  }
}
```

## Conclusion (บทสรุป)
การใช้ API ของ MindsDB ทำให้การพัฒนาโมเดลการเรียนรู้ของเครื่องเป็นไปอย่างสะดวกและรวดเร็ว คุณสามารถสร้างโมเดลและทำการพยากรณ์ได้อย่างง่ายดายผ่าน API ที่ให้บริการโดย MindsDB.