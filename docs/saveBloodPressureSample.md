# saveBloodPressureSample

Save a Blood Pressure sample to Healthkit

Example input options:

```javascript
let options = {
  bloodPressureSystolicValue: 120, 
  bloodPressureDiastolicValue: 80,
  date: (new Date(2022, 2, 29)).toISOString(),
}
```

Call the method:

```javascript
AppleHealthKit.saveBloodPressureSample((options: BloodPressureValueOptions), (err: string, results: HealthValue) => {
  if (err) {
    console.log('An error occured saving the blood pressure sample: ', err)
    return
  }
  // Blood Pressure successfully saved
})
```

Example output:

```json
1
```