---
title: educationSubmissionIndividualRecipient リソースの種類
description: '提出書類がクラス内の個人に割り当てられていることを示す educationSubmissionRecipient のサブクラスです。  '
author: dipakboyed
ms.openlocfilehash: 3447c91fe4f387508a3afdf80a7337786d46f860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318803"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="febb5-103">educationSubmissionIndividualRecipient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="febb5-103">educationSubmissionIndividualRecipient resource type</span></span>

> <span data-ttu-id="febb5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="febb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="febb5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="febb5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="febb5-106">提出書類がクラス内の個人に割り当てられていることを示す[educationSubmissionRecipient](educationsubmissionrecipient.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="febb5-106">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="febb5-107">Properties</span><span class="sxs-lookup"><span data-stu-id="febb5-107">Properties</span></span>
| <span data-ttu-id="febb5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="febb5-108">Property</span></span>     | <span data-ttu-id="febb5-109">種類</span><span class="sxs-lookup"><span data-stu-id="febb5-109">Type</span></span>   |<span data-ttu-id="febb5-110">説明</span><span class="sxs-lookup"><span data-stu-id="febb5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="febb5-111">userId</span><span class="sxs-lookup"><span data-stu-id="febb5-111">userId</span></span>|<span data-ttu-id="febb5-112">String</span><span class="sxs-lookup"><span data-stu-id="febb5-112">String</span></span>|<span data-ttu-id="febb5-113">提出書類が割り当てられているユーザーのユーザー ID です。</span><span class="sxs-lookup"><span data-stu-id="febb5-113">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="febb5-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="febb5-114">JSON representation</span></span>

<span data-ttu-id="febb5-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="febb5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->