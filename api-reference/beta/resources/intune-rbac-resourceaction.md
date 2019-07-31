---
title: resourceAction リソースの種類
description: リソースに対して許可され、許可されていないアクションのセット。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6a4f2c64ddc44349df15d118c0eddf05569101e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967631"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="0363f-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0363f-103">resourceAction resource type</span></span>

> <span data-ttu-id="0363f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0363f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0363f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0363f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0363f-106">リソースに対して許可され、許可されていないアクションのセット。</span><span class="sxs-lookup"><span data-stu-id="0363f-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="0363f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0363f-107">Properties</span></span>
|<span data-ttu-id="0363f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0363f-108">Property</span></span>|<span data-ttu-id="0363f-109">型</span><span class="sxs-lookup"><span data-stu-id="0363f-109">Type</span></span>|<span data-ttu-id="0363f-110">説明</span><span class="sxs-lookup"><span data-stu-id="0363f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0363f-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="0363f-111">allowedResourceActions</span></span>|<span data-ttu-id="0363f-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0363f-112">String collection</span></span>|<span data-ttu-id="0363f-113">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="0363f-113">Allowed Actions</span></span>|
|<span data-ttu-id="0363f-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="0363f-114">notAllowedResourceActions</span></span>|<span data-ttu-id="0363f-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0363f-115">String collection</span></span>|<span data-ttu-id="0363f-116">許可されていないアクション。</span><span class="sxs-lookup"><span data-stu-id="0363f-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0363f-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0363f-117">Relationships</span></span>
<span data-ttu-id="0363f-118">なし</span><span class="sxs-lookup"><span data-stu-id="0363f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0363f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0363f-119">JSON Representation</span></span>
<span data-ttu-id="0363f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0363f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





