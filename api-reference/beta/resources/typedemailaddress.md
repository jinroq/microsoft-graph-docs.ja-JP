---
title: typedEmailAddress リソースの種類
description: 名前、電子メール アドレス、および連絡先の対応する電子メール アドレス タイプを表します。
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510709"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="2efa7-103">typedEmailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2efa7-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2efa7-104">名前、電子メール アドレス、および、対応する電子メール アドレスの種類[にお問い合わせください](contact.md)を表します。</span><span class="sxs-lookup"><span data-stu-id="2efa7-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2efa7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2efa7-105">Properties</span></span>
| <span data-ttu-id="2efa7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2efa7-106">Property</span></span>     | <span data-ttu-id="2efa7-107">型</span><span class="sxs-lookup"><span data-stu-id="2efa7-107">Type</span></span>   |<span data-ttu-id="2efa7-108">説明</span><span class="sxs-lookup"><span data-stu-id="2efa7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2efa7-109">address</span><span class="sxs-lookup"><span data-stu-id="2efa7-109">address</span></span>|<span data-ttu-id="2efa7-110">String</span><span class="sxs-lookup"><span data-stu-id="2efa7-110">String</span></span>|<span data-ttu-id="2efa7-111">連絡先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2efa7-111">The email address of a contact.</span></span>|
|<span data-ttu-id="2efa7-112">name</span><span class="sxs-lookup"><span data-stu-id="2efa7-112">name</span></span>|<span data-ttu-id="2efa7-113">String</span><span class="sxs-lookup"><span data-stu-id="2efa7-113">String</span></span>|<span data-ttu-id="2efa7-114">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="2efa7-114">The display name of a contact.</span></span>|
|<span data-ttu-id="2efa7-115">type</span><span class="sxs-lookup"><span data-stu-id="2efa7-115">type</span></span> |<span data-ttu-id="2efa7-116">String</span><span class="sxs-lookup"><span data-stu-id="2efa7-116">String</span></span> |<span data-ttu-id="2efa7-117">電子メール アドレスの種類。</span><span class="sxs-lookup"><span data-stu-id="2efa7-117">The type of email address.</span></span> <span data-ttu-id="2efa7-118">可能な値は、`unknown`、`work`、`personal`、`main`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="2efa7-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="2efa7-119">既定値は、 `unknown`、つまり、**アドレス**が設定されていない特定の種類として。</span><span class="sxs-lookup"><span data-stu-id="2efa7-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="2efa7-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="2efa7-120">otherLabel</span></span> |<span data-ttu-id="2efa7-121">String</span><span class="sxs-lookup"><span data-stu-id="2efa7-121">String</span></span>  |<span data-ttu-id="2efa7-122">電子メール アドレスのカスタムの型を指定する**の種類**を設定`other`、 **otherLabel**を独自の文字列を割り当てるとします。</span><span class="sxs-lookup"><span data-stu-id="2efa7-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="2efa7-123">など、ボランティア活動の特定の電子メール アドレスを使用する場合があります。</span><span class="sxs-lookup"><span data-stu-id="2efa7-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="2efa7-124">**タイプ**を設定`other`、 **otherLabel**を次のように独自の文字列を設定して`Volunteer work`。</span><span class="sxs-lookup"><span data-stu-id="2efa7-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2efa7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2efa7-125">JSON representation</span></span>

<span data-ttu-id="2efa7-126">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2efa7-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
