# LunarYearDatePicker
a Swift UI component for Lunar Calendar Picker

!["ScreenShots"](/Screenshot/1.png)



Usage:
```swift
struct ContentView: View {

    @State var date = Date()

    var body: some View {
        VStack(alignment: .leading) {
            LunarDatePicker($date)
                .pickerStyle(MenuPickerStyle())

            DatePicker("國曆出生",
                       selection: $date,
                       displayedComponents: [.date])


        }.padding()
    }
}
```
a Date Picker with a Converter between Solar & Lunar Calendar
