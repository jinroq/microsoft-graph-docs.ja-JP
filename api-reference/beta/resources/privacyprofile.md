---
title: privacyProfile リソースの種類
description: 会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。
localization_priority: Normal
ms.openlocfilehash: adbd2e04e4d3898de559682b0b87158f938e7252
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833048"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="26e30-103">privacyProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26e30-103">privacyProfile resource type</span></span>

> <span data-ttu-id="26e30-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26e30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26e30-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26e30-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26e30-106">会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="26e30-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="26e30-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e30-107">Properties</span></span>
| <span data-ttu-id="26e30-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e30-108">Property</span></span>   | <span data-ttu-id="26e30-109">種類</span><span class="sxs-lookup"><span data-stu-id="26e30-109">Type</span></span>|<span data-ttu-id="26e30-110">説明</span><span class="sxs-lookup"><span data-stu-id="26e30-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26e30-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="26e30-111">contactEmail</span></span>|<span data-ttu-id="26e30-112">String</span><span class="sxs-lookup"><span data-stu-id="26e30-112">String</span></span>| <span data-ttu-id="26e30-113">プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="26e30-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="26e30-114">省略可。</span><span class="sxs-lookup"><span data-stu-id="26e30-114">Not required.</span></span>|
|<span data-ttu-id="26e30-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="26e30-115">statementUrl</span></span>|<span data-ttu-id="26e30-116">String</span><span class="sxs-lookup"><span data-stu-id="26e30-116">String</span></span>| <span data-ttu-id="26e30-117">http:// または https:// で始まる有効な URL 形式。</span><span class="sxs-lookup"><span data-stu-id="26e30-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="26e30-118">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="26e30-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="26e30-119">会社のプライバシー ステートメントに誘導する URL。</span><span class="sxs-lookup"><span data-stu-id="26e30-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="26e30-120">省略可。</span><span class="sxs-lookup"><span data-stu-id="26e30-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26e30-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26e30-121">JSON representation</span></span>

<span data-ttu-id="26e30-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="26e30-122">Here is a JSON representation of the resource</span></span>

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
