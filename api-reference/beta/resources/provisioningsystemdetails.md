---
title: 入力システムの詳細リソースの種類
description: ユーザーがプロビジョニングされたシステムを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349423"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="5c428-103">入力システムの詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c428-103">provisioningSystemDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c428-104">ユーザーがプロビジョニングされたシステムを表します。</span><span class="sxs-lookup"><span data-stu-id="5c428-104">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="5c428-105">たとえば、Azure Active Directory (Azure AD) から ServiceNow にユーザーをプロビジョニングするときに、ソースシステムが Azure AD で、ターゲットシステムが ServiceNow であるとします。</span><span class="sxs-lookup"><span data-stu-id="5c428-105">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="5c428-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c428-106">Properties</span></span>

| <span data-ttu-id="5c428-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c428-107">Property</span></span>     | <span data-ttu-id="5c428-108">型</span><span class="sxs-lookup"><span data-stu-id="5c428-108">Type</span></span>        | <span data-ttu-id="5c428-109">説明</span><span class="sxs-lookup"><span data-stu-id="5c428-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c428-110">詳細</span><span class="sxs-lookup"><span data-stu-id="5c428-110">details</span></span>|[<span data-ttu-id="5c428-111">詳細情報</span><span class="sxs-lookup"><span data-stu-id="5c428-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="5c428-112">システムの詳細。</span><span class="sxs-lookup"><span data-stu-id="5c428-112">Details of the system.</span></span>|
|<span data-ttu-id="5c428-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5c428-113">displayName</span></span>|<span data-ttu-id="5c428-114">String</span><span class="sxs-lookup"><span data-stu-id="5c428-114">String</span></span>|<span data-ttu-id="5c428-115">ユーザーがプロビジョニングされたシステムの名前。</span><span class="sxs-lookup"><span data-stu-id="5c428-115">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="5c428-116">id</span><span class="sxs-lookup"><span data-stu-id="5c428-116">id</span></span>|<span data-ttu-id="5c428-117">文字列</span><span class="sxs-lookup"><span data-stu-id="5c428-117">String</span></span>|<span data-ttu-id="5c428-118">ユーザーがプロビジョニングされたシステムの識別子。</span><span class="sxs-lookup"><span data-stu-id="5c428-118">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c428-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c428-119">JSON representation</span></span>

<span data-ttu-id="5c428-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c428-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
