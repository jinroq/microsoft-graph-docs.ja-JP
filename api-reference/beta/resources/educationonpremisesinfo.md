---
title: educationOnPremisesInfo リソースの種類
description: オンプレミスの Active Directory ユーザーアカウントを Azure AD ユーザーオブジェクトに関連付けるために使用される追加情報。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764771"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="2cc80-103">educationOnPremisesInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cc80-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="2cc80-104">オンプレミスの Active Directory ユーザーアカウントを Azure AD ユーザーオブジェクトに関連付けるために使用される追加情報。</span><span class="sxs-lookup"><span data-stu-id="2cc80-104">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="2cc80-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cc80-105">Properties</span></span>

| <span data-ttu-id="2cc80-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cc80-106">Property</span></span>    | <span data-ttu-id="2cc80-107">型</span><span class="sxs-lookup"><span data-stu-id="2cc80-107">Type</span></span>   | <span data-ttu-id="2cc80-108">説明</span><span class="sxs-lookup"><span data-stu-id="2cc80-108">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="2cc80-109">immutableId</span><span class="sxs-lookup"><span data-stu-id="2cc80-109">immutableId</span></span> | <span data-ttu-id="2cc80-110">String</span><span class="sxs-lookup"><span data-stu-id="2cc80-110">String</span></span> | <span data-ttu-id="2cc80-111">Active Directory 内のユーザーオブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2cc80-111">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2cc80-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cc80-112">JSON representation</span></span>

<span data-ttu-id="2cc80-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cc80-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
