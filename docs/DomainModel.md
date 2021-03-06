# GoEthi domain models

## Main concepts model

![GoEthi main concepts model](http://yuml.me/diagram/scruffy/class/[Product]*-[Manufacturer],[Owner]-*[Manufacturer],[Owner]-0..*[Owner],[Manufacturer]-0..*[Owner],[Product]++-1[ProductIdentity],[User]-0..*[UserDevice],[User]-0..*[MoralValues],[Behavior]*-[User],[Brand]-1..*[Owner],[ProductIdentity]-[note:e.g. barcode{bg:wheat}],[Institution]^-[Owner],[Institution]^-[Manufacturer],[ProductCategory]-[note:e.g. based on Google Product Category{bg:wheat}],[ProductCategory]-[Product],[Product]-[Brand],[Address]*-[User],[Institution]-*[Address] "GoEthi Main concepts model")

## User behavior model

![GoEthi behavior domain model](http://yuml.me/diagram/scruffy;dir:BT/class/[Behavior]*-[User],[ProductRelatedBehavior]-^[Behavior],[Behavior]-[note:on hehalf of the user geolocalized and possibly associated with device{bg:wheat}],[ProductIdentificationBehavior]-^[Behavior],[ProductIdentificationBehavior]-.-^[<<ProductRelatedBehavior>>],[ProductDenialBehavior]-^[Behavior],[ProductDenialBehavior]-.-^[<<ProductRelatedBehavior>>],[AddProductIntentBehavior]-^[ProductRelatedBehavior],[EditProductIntentBehavior]-.-^[<<ProductRelatedBehavior>>],[EditOwnerBehavior]-^[Behavior],[EditOwnerBehavior]-.-^[<<OwnerRelatedBehavior>>],[AddProductOwnerBehavior]-^[Behavior],[AddProductOwnerBehavior]-.-^[<<ProductRelatedBehavior>>],[AddProductOwnerBehavior]-.-^[<<OwnerRelatedBehavior>>] "GoEthi behavior domain model")
