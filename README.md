# Task for Frontend Engineer

The following document describes the requirements, resources and expectations related
to the task for the JavaScript Engineer role.

**Please read it carefully to better understand what we are asking for and
what we expect from you.
After you done please share the codesandbox link to whom in may concern.
Should you have any question after reading this document, please do not
hesitate to contact us.**

The requirements for this task we ask you to create a SPA using **ReactJS**.

The application must meet the following requirements:

- Fetch all available cars
- Implement pagination with limit of 10
- Allow the user to filter the cars by manufacturer or color.
- Allow the user to sort the car by mileage.
- Show the details of a selected car.
- Add/Remove a car to/from the favorites collection using local storage.

# Resources

For the UI, please use the attached design and style guide as a visual guide for your
application and implement the styles yourself from scratch instead of using a library
like Bootstrap or Material UI.

For the cars data, please use the

`axios({ url: '/api/cars?page=1&sort=desc&manufacturer=Audi&color=red' })` to fetch cars

```javascript
{
  cars: [
    stockNumber: 12345,
    manufacturerName: 'Audi',
    modelName: 'A5',
    color: 'red',
    mileage: {
      number: 223;
      unit: 1;
    },
    fuelType: 'Benzin',
    pictureUrl: '/images/car.svg'
  ],
  totalPageCount: 20,
  totalCarsCount: 100
}
```

`axios({ url: '/api/cars/1' })` to fetch one car by stockNumber
`axios({ url: '/api/colors' })` to fetch colors
`axios({ url: '/api/manufacturers' })` to fetch manufacturers

# Our expectations

The most important things for us when evaluating your solution are:

- Best practices
- Clear code organization and project structure
- A well developed UI/UX
- Good unit testing coverage

Feel free to choose the techniques you feel more comfortable with and
the most important thing: _Have fun!_
