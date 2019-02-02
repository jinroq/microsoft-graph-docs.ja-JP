---
title: relatedContact リソースの種類
description: 守護者、援助施設、医師というように情報を提供する、educationUser に関連するレコードにお問い合わせください。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694490"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="e1d7e-103">realtedContact リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1d7e-103">realtedContact resource type</span></span>

<span data-ttu-id="e1d7e-104">守護者、援助施設、医師というように情報を提供する[educationUser](../resources/educationuser.md)に関連するレコードにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="e1d7e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1d7e-105">Properties</span></span>
| <span data-ttu-id="e1d7e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1d7e-106">Property</span></span>     | <span data-ttu-id="e1d7e-107">型</span><span class="sxs-lookup"><span data-stu-id="e1d7e-107">Type</span></span>   |<span data-ttu-id="e1d7e-108">説明</span><span class="sxs-lookup"><span data-stu-id="e1d7e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1d7e-109">id</span><span class="sxs-lookup"><span data-stu-id="e1d7e-109">id</span></span>|<span data-ttu-id="e1d7e-110">String</span><span class="sxs-lookup"><span data-stu-id="e1d7e-110">String</span></span>|<span data-ttu-id="e1d7e-111">Azure Active Directory 内の連絡先の id。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="e1d7e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e1d7e-112">displayName</span></span>|<span data-ttu-id="e1d7e-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e1d7e-113">String</span></span>|<span data-ttu-id="e1d7e-114">連絡先の名前です。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-114">Name of the contact.</span></span> <span data-ttu-id="e1d7e-115">必須。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-115">Required.</span></span>|
|<span data-ttu-id="e1d7e-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e1d7e-116">emailAddress</span></span>|<span data-ttu-id="e1d7e-117">String</span><span class="sxs-lookup"><span data-stu-id="e1d7e-117">String</span></span>|<span data-ttu-id="e1d7e-118">連絡先のプライマリ電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="e1d7e-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e1d7e-119">mobilePhone</span></span>|<span data-ttu-id="e1d7e-120">String</span><span class="sxs-lookup"><span data-stu-id="e1d7e-120">String</span></span>|<span data-ttu-id="e1d7e-121">連絡先の携帯電話番号です。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="e1d7e-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1d7e-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="e1d7e-123">ユーザーに関係します。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-123">Relationship to the user.</span></span> <span data-ttu-id="e1d7e-124">使用可能な値は、 `parent`、 `relative`、 `aide`、 `doctor`、 `guardian`、 `child`、 `other`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e1d7e-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="e1d7e-125">accessConsent</span></span>|<span data-ttu-id="e1d7e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1d7e-126">Boolean</span></span>|<span data-ttu-id="e1d7e-127">受講者用のデータにアクセスするユーザーが同意したされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1d7e-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1d7e-128">JSON representation</span></span>

<span data-ttu-id="e1d7e-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1d7e-129">The following is a JSON representation of the resource.</span></span>

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
