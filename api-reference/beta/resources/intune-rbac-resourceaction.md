---
title: resourceAction リソースの種類
description: リソースに対して許可され、許可されていないアクションのセット。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4cccb0b47d0d4724ebba7a4749529ccbfe5f7f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566340"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="9fb3c-103">resourceAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9fb3c-103">resourceAction resource type</span></span>

> <span data-ttu-id="9fb3c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fb3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fb3c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9fb3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fb3c-106">リソースに対して許可され、許可されていないアクションのセット。</span><span class="sxs-lookup"><span data-stu-id="9fb3c-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9fb3c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fb3c-107">Properties</span></span>
|<span data-ttu-id="9fb3c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fb3c-108">Property</span></span>|<span data-ttu-id="9fb3c-109">型</span><span class="sxs-lookup"><span data-stu-id="9fb3c-109">Type</span></span>|<span data-ttu-id="9fb3c-110">説明</span><span class="sxs-lookup"><span data-stu-id="9fb3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fb3c-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="9fb3c-111">allowedResourceActions</span></span>|<span data-ttu-id="9fb3c-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9fb3c-112">String collection</span></span>|<span data-ttu-id="9fb3c-113">許可されるアクション</span><span class="sxs-lookup"><span data-stu-id="9fb3c-113">Allowed Actions</span></span>|
|<span data-ttu-id="9fb3c-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="9fb3c-114">notAllowedResourceActions</span></span>|<span data-ttu-id="9fb3c-115">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9fb3c-115">String collection</span></span>|<span data-ttu-id="9fb3c-116">許可されていないアクション。</span><span class="sxs-lookup"><span data-stu-id="9fb3c-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fb3c-117">関係</span><span class="sxs-lookup"><span data-stu-id="9fb3c-117">Relationships</span></span>
<span data-ttu-id="9fb3c-118">なし</span><span class="sxs-lookup"><span data-stu-id="9fb3c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fb3c-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9fb3c-119">JSON Representation</span></span>
<span data-ttu-id="9fb3c-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9fb3c-120">Here is a JSON representation of the resource.</span></span>
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





