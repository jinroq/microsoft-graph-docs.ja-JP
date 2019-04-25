---
title: その他の連絡先リソースの種類
description: 保護者、支援、医師などの情報を提供する educationUser に関連する連絡先レコード。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579409"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="30cb4-103">realtedcontact リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30cb4-103">realtedContact resource type</span></span>

<span data-ttu-id="30cb4-104">保護者、支援、医師などの情報を提供する[educationUser](../resources/educationuser.md)に関連する連絡先レコード。</span><span class="sxs-lookup"><span data-stu-id="30cb4-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="30cb4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30cb4-105">Properties</span></span>
| <span data-ttu-id="30cb4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30cb4-106">Property</span></span>     | <span data-ttu-id="30cb4-107">型</span><span class="sxs-lookup"><span data-stu-id="30cb4-107">Type</span></span>   |<span data-ttu-id="30cb4-108">説明</span><span class="sxs-lookup"><span data-stu-id="30cb4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30cb4-109">id</span><span class="sxs-lookup"><span data-stu-id="30cb4-109">id</span></span>|<span data-ttu-id="30cb4-110">String</span><span class="sxs-lookup"><span data-stu-id="30cb4-110">String</span></span>|<span data-ttu-id="30cb4-111">Azure Active Directory 内の連絡先の id。</span><span class="sxs-lookup"><span data-stu-id="30cb4-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="30cb4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="30cb4-112">displayName</span></span>|<span data-ttu-id="30cb4-113">String</span><span class="sxs-lookup"><span data-stu-id="30cb4-113">String</span></span>|<span data-ttu-id="30cb4-114">連絡先の名前。</span><span class="sxs-lookup"><span data-stu-id="30cb4-114">Name of the contact.</span></span> <span data-ttu-id="30cb4-115">必須です。</span><span class="sxs-lookup"><span data-stu-id="30cb4-115">Required.</span></span>|
|<span data-ttu-id="30cb4-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="30cb4-116">emailAddress</span></span>|<span data-ttu-id="30cb4-117">String</span><span class="sxs-lookup"><span data-stu-id="30cb4-117">String</span></span>|<span data-ttu-id="30cb4-118">連絡先のプライマリ電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="30cb4-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="30cb4-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="30cb4-119">mobilePhone</span></span>|<span data-ttu-id="30cb4-120">String</span><span class="sxs-lookup"><span data-stu-id="30cb4-120">String</span></span>|<span data-ttu-id="30cb4-121">連絡先の携帯電話番号。</span><span class="sxs-lookup"><span data-stu-id="30cb4-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="30cb4-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="30cb4-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="30cb4-123">ユーザーとの関係。</span><span class="sxs-lookup"><span data-stu-id="30cb4-123">Relationship to the user.</span></span> <span data-ttu-id="30cb4-124">可能な値`parent`は`relative` `aide` `doctor` `guardian` `other`、、、、、、 `unknownFutureValue`、、です。 `child`</span><span class="sxs-lookup"><span data-stu-id="30cb4-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="30cb4-125">accessconsent</span><span class="sxs-lookup"><span data-stu-id="30cb4-125">accessConsent</span></span>|<span data-ttu-id="30cb4-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="30cb4-126">Boolean</span></span>|<span data-ttu-id="30cb4-127">ユーザーが学生データにアクセスするために同意されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="30cb4-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30cb4-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30cb4-128">JSON representation</span></span>

<span data-ttu-id="30cb4-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30cb4-129">The following is a JSON representation of the resource.</span></span>

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
