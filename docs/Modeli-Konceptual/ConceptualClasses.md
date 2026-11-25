# RentTools - Klasat koncetuale

## 1.Costumer

Përfaqëson klientin që përdor sistemin për rezervimet e veglave.

Atributet:
-CostumerId
-fistName
-lastName
-email
-phoneNumber

## 2.Tool
Përfaqëson një lloj vegle që ofrohet për dhënie me qira.

Atributet:
-toolId
-name
-description
-category
-dailyPrice

## 3.ToolUnit
Përfaqëson një njësi fizike të veglës.

Atributet:
-unitId
-serialNumber
-condition
-status

## 4. Maintenance
Përfaqëson mirëmbajtjen dhe servisimin e një njësie të veglës.

Atributet:
-maintenanceId
-startDate
-endDate
-description
-cost
-status

## 5.Reservation
Përfaqëson rezervimin e krijuar nga një klient.

Atributet:
-reservationId
-creationId
-startDate
-endDate
-status

## 6.ReservationItem
Përfaqëson një njësi vegle brenda një rezervimi.

Kjo klasë mundëson rezervimin edisa veglave në një rezervim të vetëm.

Atributet:
-itemId
-dailyPrice
-subtotal

## 7.Rental
Përfaqëson procesin e dhënjes me qira të veglave të rezervuara.

Atributet:
-rentalId
-pickupDate
-expectedReturnDate
-status

## 8.Return
Përfaqëson kthimin e një njësie te veglës dhe kontrollin e gjendjes.

Atributet:
-returnId
-returnDate
-toolConditon
-damageDescription
  
## 9.Invoice
Përfaqëson faturen e krijuar për një qira.

Atributet:
-invoiceId
-issueDate
-rentalAmount
-lateFee
-damageFee
-totalAmount
-status

## 10.Payment 
Përfaqëson pagesen e realizuar nga klijenti.

Atributet:
-PaymentId
-paymentDate
-amount
-paymentMethod
-status

## Ndarja sipas moduleve

### Inventory & Availability
-Tool
-ToolUnit
-Maintenance

### Booking Menagement
-Costumer
-Reservation
-ReservaionItem

### Rental & Returns
-Rental
-Return

### Billing & Payments
-InVoice
-Payment

Mardheniet ndermjet klasave dhe multiplicitetet do te percaktohen ne diagramin konceptual UML.
