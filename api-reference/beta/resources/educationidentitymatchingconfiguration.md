---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520313"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="5d6e0-105">educationIdentityMatchingConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d6e0-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d6e0-106">学校のデータのプロファイルの id を一致させるための設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="5d6e0-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="5d6e0-107">これらの id には、生徒と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5d6e0-107">These identities include students and teachers.</span></span> <span data-ttu-id="5d6e0-108">これらの設定に基づいて、ユーザーがディレクトリで更新されます。</span><span class="sxs-lookup"><span data-stu-id="5d6e0-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="5d6e0-109">**注:** このリソースが選択されている場合は、ユーザーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="5d6e0-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="5d6e0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d6e0-110">Properties</span></span>

| <span data-ttu-id="5d6e0-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d6e0-111">Property</span></span> | <span data-ttu-id="5d6e0-112">型</span><span class="sxs-lookup"><span data-stu-id="5d6e0-112">Type</span></span> | <span data-ttu-id="5d6e0-113">説明</span><span class="sxs-lookup"><span data-stu-id="5d6e0-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5d6e0-114">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="5d6e0-114">**matchingOptions**</span></span> | <span data-ttu-id="5d6e0-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5d6e0-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="5d6e0-116">ユーザー アカウントを更新するユーザーを一意に識別に使用するオプションの間のマッピングです。</span><span class="sxs-lookup"><span data-stu-id="5d6e0-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d6e0-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d6e0-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
