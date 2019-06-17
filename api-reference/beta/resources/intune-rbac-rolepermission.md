---
title: rolePermission リソースの種類
description: 各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cbe41bae81d165d0800a5184e1f7babedebc09d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993523"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="66195-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66195-103">rolePermission resource type</span></span>

> <span data-ttu-id="66195-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66195-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66195-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66195-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66195-106">各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="66195-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="66195-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66195-107">Properties</span></span>
|<span data-ttu-id="66195-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66195-108">Property</span></span>|<span data-ttu-id="66195-109">型</span><span class="sxs-lookup"><span data-stu-id="66195-109">Type</span></span>|<span data-ttu-id="66195-110">説明</span><span class="sxs-lookup"><span data-stu-id="66195-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66195-111">actions</span><span class="sxs-lookup"><span data-stu-id="66195-111">actions</span></span>|<span data-ttu-id="66195-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="66195-112">String collection</span></span>|<span data-ttu-id="66195-113">許可されたアクション-非推奨</span><span class="sxs-lookup"><span data-stu-id="66195-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="66195-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="66195-114">resourceActions</span></span>|<span data-ttu-id="66195-115">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="66195-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="66195-116">それぞれ許可され、許可されていないアクセス許可のセットが含まれているリソースアクション。</span><span class="sxs-lookup"><span data-stu-id="66195-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66195-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66195-117">Relationships</span></span>
<span data-ttu-id="66195-118">なし</span><span class="sxs-lookup"><span data-stu-id="66195-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66195-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66195-119">JSON Representation</span></span>
<span data-ttu-id="66195-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66195-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```





