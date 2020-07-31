---
title: Iconography
---
import {DoDontContainer, Do, Dont, Caption} from '@primer/gatsby-theme-doctocat'
import Iconography1 from '../../src/images/Iconography-1.png'
import Iconography2 from '../../src/images/Iconography-2.png'
import Iconography3 from '../../src/images/Iconography-3.png'
import Iconography4 from '../../src/images/Iconography-4.png'

While CLI does not have images, we do have unicode at our disposal to enhance meaning. When applying iconography consider:

- People use different fonts that will have varying unicode support
- Only use iconography to enhance meaning, not to communicate meaning
  - ref: https://primer.style/design/global/accessibility#visual-accessibility
  - Similar to using iconography in general!

_Note: In Windows, Powershell’s default font (Lucida Console) has poor unicode support. Microsoft suggests changing it for more unicode support._

**Symbols currently used:**
```
✓ 	Success
- 	Neutral
✗   Failure
+ 	Changes requested
! 	Alert
```

<DoDontContainer>
  <Do src={Iconography1}>
    Use checks for success messages
  </Do>
  <Dont src={Iconography2}>
    Don't use checks for failure messages
  </Dont>
</DoDontContainer>

<DoDontContainer>
  <Do src={Iconography3}>
    Use checks for success of closing or deleting
  </Do>
  <Dont src={Iconography4}>
    Don't use alerts when closing or deleting
  </Dont>
</DoDontContainer>
