---
title: 開始側リソースの種類
description: プロビジョニングイベントを開始したユーザーまたは対象について説明します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2846c247d4a0d196d4c620f447b40d47cd486c81
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349430"
---
# <a name="initiator-resource-type"></a><span data-ttu-id="d9242-103">開始側リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9242-103">initiator resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9242-104">プロビジョニングイベントを開始したユーザーまたは対象について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9242-104">Describes who or what initiated the provisioning event.</span></span> 

## <a name="properties"></a><span data-ttu-id="d9242-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9242-105">Properties</span></span>

| <span data-ttu-id="d9242-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9242-106">Property</span></span>     | <span data-ttu-id="d9242-107">型</span><span class="sxs-lookup"><span data-stu-id="d9242-107">Type</span></span>        | <span data-ttu-id="d9242-108">説明</span><span class="sxs-lookup"><span data-stu-id="d9242-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9242-109">displayName</span><span class="sxs-lookup"><span data-stu-id="d9242-109">displayName</span></span>|<span data-ttu-id="d9242-110">String</span><span class="sxs-lookup"><span data-stu-id="d9242-110">String</span></span>|<span data-ttu-id="d9242-111">プロビジョニングイベントを開始したユーザーまたはサービスの名前。</span><span class="sxs-lookup"><span data-stu-id="d9242-111">Name of the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="d9242-112">id</span><span class="sxs-lookup"><span data-stu-id="d9242-112">id</span></span>|<span data-ttu-id="d9242-113">文字列</span><span class="sxs-lookup"><span data-stu-id="d9242-113">String</span></span>|<span data-ttu-id="d9242-114">プロビジョニングイベントを開始した個人またはサービスを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="d9242-114">Uniquely identifies the person or service that initiated the provisioning event.</span></span>|
|<span data-ttu-id="d9242-115">initiatorType</span><span class="sxs-lookup"><span data-stu-id="d9242-115">initiatorType</span></span>|<span data-ttu-id="d9242-116">String</span><span class="sxs-lookup"><span data-stu-id="d9242-116">String</span></span>| <span data-ttu-id="d9242-117">イニシエーターの種類。</span><span class="sxs-lookup"><span data-stu-id="d9242-117">Type of initiator.</span></span> <span data-ttu-id="d9242-118">使用可能な値は、`user`、`app`、`system`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="d9242-118">Possible values are: `user`, `app`, `system`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9242-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9242-119">JSON representation</span></span>

<span data-ttu-id="d9242-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d9242-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
