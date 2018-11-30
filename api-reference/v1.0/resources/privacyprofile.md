---
title: privacyProfile リソースの種類
description: 会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。
ms.openlocfilehash: 5d1a8e48a2d8310f45c71fbc73485e8ec4fe8697
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023693"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="d54d9-103">privacyProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d54d9-103">privacyProfile resource type</span></span>

<span data-ttu-id="d54d9-104">会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d54d9-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="d54d9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d54d9-105">Properties</span></span>
| <span data-ttu-id="d54d9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d54d9-106">Property</span></span>   | <span data-ttu-id="d54d9-107">型</span><span class="sxs-lookup"><span data-stu-id="d54d9-107">Type</span></span>|<span data-ttu-id="d54d9-108">説明</span><span class="sxs-lookup"><span data-stu-id="d54d9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d54d9-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="d54d9-109">contactEmail</span></span>|<span data-ttu-id="d54d9-110">String</span><span class="sxs-lookup"><span data-stu-id="d54d9-110">String</span></span>| <span data-ttu-id="d54d9-111">プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="d54d9-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="d54d9-112">省略可。</span><span class="sxs-lookup"><span data-stu-id="d54d9-112">Not required.</span></span>|
|<span data-ttu-id="d54d9-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="d54d9-113">statementUrl</span></span>|<span data-ttu-id="d54d9-114">String</span><span class="sxs-lookup"><span data-stu-id="d54d9-114">String</span></span>| <span data-ttu-id="d54d9-115">http:// または https:// で始まる有効な URL 形式。</span><span class="sxs-lookup"><span data-stu-id="d54d9-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="d54d9-116">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="d54d9-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="d54d9-117">会社のプライバシー ステートメントに誘導する URL。</span><span class="sxs-lookup"><span data-stu-id="d54d9-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="d54d9-118">省略可。</span><span class="sxs-lookup"><span data-stu-id="d54d9-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d54d9-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d54d9-119">JSON representation</span></span>

<span data-ttu-id="d54d9-120">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="d54d9-120">Here is a JSON representation of the resource</span></span>

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