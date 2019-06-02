---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 357f47f549e96b0f7c7ce0ecec4b5c791b5d3897
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = new EducationSchool
{
    DisplayName = "Fabrikam High School",
    Description = "Magnate school for the arts. Los Angeles School District",
    Status = "String",
    ExternalSource = EducationExternalSource.Sis,
    PrincipalEmail = "AmyR@fabrikam.com",
    PrincipalName = "Amy Roebuck",
    ExternalPrincipalId = "14007",
    HighestGrade = "12",
    LowestGrade = "9",
    SchoolNumber = "10002",
    Address = new PhysicalAddress
    {
        City = "Los Angeles",
        CountryOrRegion = "United States",
        PostalCode = "98055",
        State = "CA",
        Street = "12345 Main St."
    },
    ExternalId = "10002",
    Fax = "+1 (253) 555-0101",
    Phone = "+1 (253) 555-0102"
};

await graphClient.Education.Schools
    .Request()
    .AddAsync(educationSchool);

```