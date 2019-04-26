---
title: privacyProfile リソースの種類
description: 会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。
localization_priority: Normal
ms.openlocfilehash: d1d7593e5b0f0ef9d4ac36f902ec244e93fd51c1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344203"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="876a6-103">privacyProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="876a6-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="876a6-104">会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="876a6-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="876a6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="876a6-105">Properties</span></span>
| <span data-ttu-id="876a6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="876a6-106">Property</span></span>   | <span data-ttu-id="876a6-107">型</span><span class="sxs-lookup"><span data-stu-id="876a6-107">Type</span></span>|<span data-ttu-id="876a6-108">説明</span><span class="sxs-lookup"><span data-stu-id="876a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="876a6-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="876a6-109">contactEmail</span></span>|<span data-ttu-id="876a6-110">String</span><span class="sxs-lookup"><span data-stu-id="876a6-110">String</span></span>| <span data-ttu-id="876a6-111">プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="876a6-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="876a6-112">省略可。</span><span class="sxs-lookup"><span data-stu-id="876a6-112">Not required.</span></span>|
|<span data-ttu-id="876a6-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="876a6-113">statementUrl</span></span>|<span data-ttu-id="876a6-114">String</span><span class="sxs-lookup"><span data-stu-id="876a6-114">String</span></span>| <span data-ttu-id="876a6-115">http:// または https:// で始まる有効な URL 形式。</span><span class="sxs-lookup"><span data-stu-id="876a6-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="876a6-116">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="876a6-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="876a6-117">会社のプライバシー ステートメントに誘導する URL。</span><span class="sxs-lookup"><span data-stu-id="876a6-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="876a6-118">省略可。</span><span class="sxs-lookup"><span data-stu-id="876a6-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="876a6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="876a6-119">JSON representation</span></span>

<span data-ttu-id="876a6-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="876a6-120">Here is a JSON representation of the resource</span></span>

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
