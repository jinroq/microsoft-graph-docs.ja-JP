---
title: rolePermission リソースの種類
description: 各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3fadd331cfb0e8201dcc77abe066d1c2c0b1c2c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010575"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="6515f-103">rolePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6515f-103">rolePermission resource type</span></span>

> <span data-ttu-id="6515f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6515f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6515f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6515f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6515f-106">各役割に対して許可されるアクセス許可と許可されないアクセス許可を決定する ResourceActions のセットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6515f-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="6515f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6515f-107">Properties</span></span>
|<span data-ttu-id="6515f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6515f-108">Property</span></span>|<span data-ttu-id="6515f-109">型</span><span class="sxs-lookup"><span data-stu-id="6515f-109">Type</span></span>|<span data-ttu-id="6515f-110">説明</span><span class="sxs-lookup"><span data-stu-id="6515f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6515f-111">actions</span><span class="sxs-lookup"><span data-stu-id="6515f-111">actions</span></span>|<span data-ttu-id="6515f-112">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6515f-112">String collection</span></span>|<span data-ttu-id="6515f-113">許可されたアクション-非推奨</span><span class="sxs-lookup"><span data-stu-id="6515f-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="6515f-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="6515f-114">resourceActions</span></span>|<span data-ttu-id="6515f-115">[resourceAction](../resources/intune-rbac-resourceaction.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6515f-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="6515f-116">それぞれ許可され、許可されていないアクセス許可のセットが含まれているリソースアクション。</span><span class="sxs-lookup"><span data-stu-id="6515f-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6515f-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6515f-117">Relationships</span></span>
<span data-ttu-id="6515f-118">なし</span><span class="sxs-lookup"><span data-stu-id="6515f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6515f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6515f-119">JSON Representation</span></span>
<span data-ttu-id="6515f-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6515f-120">Here is a JSON representation of the resource.</span></span>
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





