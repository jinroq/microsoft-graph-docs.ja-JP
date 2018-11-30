---
title: privacyProfile リソースの種類
description: 会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。
ms.openlocfilehash: fb9d5f929f1c9ae28687b80e987dc0909387f5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074100"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="dec68-103">privacyProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dec68-103">privacyProfile resource type</span></span>

> <span data-ttu-id="dec68-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dec68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dec68-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dec68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dec68-106">会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="dec68-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="dec68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dec68-107">Properties</span></span>
| <span data-ttu-id="dec68-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dec68-108">Property</span></span>   | <span data-ttu-id="dec68-109">型</span><span class="sxs-lookup"><span data-stu-id="dec68-109">Type</span></span>|<span data-ttu-id="dec68-110">説明</span><span class="sxs-lookup"><span data-stu-id="dec68-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dec68-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="dec68-111">contactEmail</span></span>|<span data-ttu-id="dec68-112">String</span><span class="sxs-lookup"><span data-stu-id="dec68-112">String</span></span>| <span data-ttu-id="dec68-113">プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="dec68-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="dec68-114">省略可。</span><span class="sxs-lookup"><span data-stu-id="dec68-114">Not required.</span></span>|
|<span data-ttu-id="dec68-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="dec68-115">statementUrl</span></span>|<span data-ttu-id="dec68-116">String</span><span class="sxs-lookup"><span data-stu-id="dec68-116">String</span></span>| <span data-ttu-id="dec68-117">http:// または https:// で始まる有効な URL 形式。</span><span class="sxs-lookup"><span data-stu-id="dec68-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="dec68-118">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="dec68-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="dec68-119">会社のプライバシー ステートメントに誘導する URL。</span><span class="sxs-lookup"><span data-stu-id="dec68-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="dec68-120">省略可。</span><span class="sxs-lookup"><span data-stu-id="dec68-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dec68-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dec68-121">JSON representation</span></span>

<span data-ttu-id="dec68-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dec68-122">Here is a JSON representation of the resource</span></span>

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