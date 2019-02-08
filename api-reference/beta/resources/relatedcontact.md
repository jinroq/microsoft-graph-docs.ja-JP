---
title: relatedContact リソースの種類
description: 守護者、援助施設、医師というように情報を提供する、educationUser に関連するレコードにお問い合わせください。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694476"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="024f2-103">relatedContact リソースの種類</span><span class="sxs-lookup"><span data-stu-id="024f2-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="024f2-104">守護者、援助施設、医師というように情報を提供する[educationUser](../resources/educationuser.md)に関連するレコードにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="024f2-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="024f2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="024f2-105">Properties</span></span>
| <span data-ttu-id="024f2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="024f2-106">Property</span></span>     | <span data-ttu-id="024f2-107">型</span><span class="sxs-lookup"><span data-stu-id="024f2-107">Type</span></span>   |<span data-ttu-id="024f2-108">説明</span><span class="sxs-lookup"><span data-stu-id="024f2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="024f2-109">id</span><span class="sxs-lookup"><span data-stu-id="024f2-109">id</span></span>|<span data-ttu-id="024f2-110">String</span><span class="sxs-lookup"><span data-stu-id="024f2-110">String</span></span>|<span data-ttu-id="024f2-111">Azure Active Directory 内の連絡先の id。</span><span class="sxs-lookup"><span data-stu-id="024f2-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="024f2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="024f2-112">displayName</span></span>|<span data-ttu-id="024f2-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="024f2-113">String</span></span>|<span data-ttu-id="024f2-114">連絡先の名前です。</span><span class="sxs-lookup"><span data-stu-id="024f2-114">Name of the contact.</span></span> <span data-ttu-id="024f2-115">必須です。</span><span class="sxs-lookup"><span data-stu-id="024f2-115">Required.</span></span>|
|<span data-ttu-id="024f2-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="024f2-116">emailAddress</span></span>|<span data-ttu-id="024f2-117">String</span><span class="sxs-lookup"><span data-stu-id="024f2-117">String</span></span>|<span data-ttu-id="024f2-118">連絡先のプライマリ電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="024f2-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="024f2-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="024f2-119">mobilePhone</span></span>|<span data-ttu-id="024f2-120">String</span><span class="sxs-lookup"><span data-stu-id="024f2-120">String</span></span>|<span data-ttu-id="024f2-121">連絡先の携帯電話番号です。</span><span class="sxs-lookup"><span data-stu-id="024f2-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="024f2-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="024f2-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="024f2-123">ユーザーに関係します。</span><span class="sxs-lookup"><span data-stu-id="024f2-123">Relationship to the user.</span></span> <span data-ttu-id="024f2-124">使用可能な値は、 `parent`、 `relative`、 `aide`、 `doctor`、 `guardian`、 `child`、 `other`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="024f2-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="024f2-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="024f2-125">accessConsent</span></span>|<span data-ttu-id="024f2-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="024f2-126">Boolean</span></span>|<span data-ttu-id="024f2-127">受講者用のデータにアクセスするユーザーが同意したされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="024f2-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="024f2-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="024f2-128">JSON representation</span></span>

<span data-ttu-id="024f2-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="024f2-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
