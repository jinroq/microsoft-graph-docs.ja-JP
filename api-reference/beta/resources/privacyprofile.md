---
title: privacyProfile リソースの種類
description: 会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510121"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="2add6-103">privacyProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2add6-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2add6-104">会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2add6-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="2add6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2add6-105">Properties</span></span>
| <span data-ttu-id="2add6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2add6-106">Property</span></span>   | <span data-ttu-id="2add6-107">型</span><span class="sxs-lookup"><span data-stu-id="2add6-107">Type</span></span>|<span data-ttu-id="2add6-108">説明</span><span class="sxs-lookup"><span data-stu-id="2add6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2add6-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="2add6-109">contactEmail</span></span>|<span data-ttu-id="2add6-110">String</span><span class="sxs-lookup"><span data-stu-id="2add6-110">String</span></span>| <span data-ttu-id="2add6-111">プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2add6-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="2add6-112">省略可。</span><span class="sxs-lookup"><span data-stu-id="2add6-112">Not required.</span></span>|
|<span data-ttu-id="2add6-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="2add6-113">statementUrl</span></span>|<span data-ttu-id="2add6-114">String</span><span class="sxs-lookup"><span data-stu-id="2add6-114">String</span></span>| <span data-ttu-id="2add6-115">http:// または https:// で始まる有効な URL 形式。</span><span class="sxs-lookup"><span data-stu-id="2add6-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="2add6-116">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="2add6-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="2add6-117">会社のプライバシー ステートメントに誘導する URL。</span><span class="sxs-lookup"><span data-stu-id="2add6-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="2add6-118">省略可。</span><span class="sxs-lookup"><span data-stu-id="2add6-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2add6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2add6-119">JSON representation</span></span>

<span data-ttu-id="2add6-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2add6-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
