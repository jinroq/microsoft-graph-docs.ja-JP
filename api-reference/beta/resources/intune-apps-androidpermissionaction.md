---
title: androidpermissionaction リソースの種類
description: android アプリのアクセス許可と android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fec33b2600e88e6a4dfae644c335d9652c20abe0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792966"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="b0fdc-103">androidpermissionaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0fdc-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="b0fdc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0fdc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fdc-106">android アプリのアクセス許可と android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="b0fdc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0fdc-107">Properties</span></span>
|<span data-ttu-id="b0fdc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0fdc-108">Property</span></span>|<span data-ttu-id="b0fdc-109">型</span><span class="sxs-lookup"><span data-stu-id="b0fdc-109">Type</span></span>|<span data-ttu-id="b0fdc-110">説明</span><span class="sxs-lookup"><span data-stu-id="b0fdc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fdc-111">権</span><span class="sxs-lookup"><span data-stu-id="b0fdc-111">permission</span></span>|<span data-ttu-id="b0fdc-112">文字列</span><span class="sxs-lookup"><span data-stu-id="b0fdc-112">String</span></span>|<span data-ttu-id="b0fdc-113">android のアクセス許可文字列。公式の android ドキュメントで定義されています。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="b0fdc-114">例 ' READ_CONTACTS '。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="b0fdc-115">アクション</span><span class="sxs-lookup"><span data-stu-id="b0fdc-115">action</span></span>|[<span data-ttu-id="b0fdc-116">androidpermissionactiontype</span><span class="sxs-lookup"><span data-stu-id="b0fdc-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="b0fdc-117">Android のアクセス許可アクションの種類。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-117">Type of Android permission action.</span></span> <span data-ttu-id="b0fdc-118">可能な値は、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0fdc-119">関係</span><span class="sxs-lookup"><span data-stu-id="b0fdc-119">Relationships</span></span>
<span data-ttu-id="b0fdc-120">なし</span><span class="sxs-lookup"><span data-stu-id="b0fdc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0fdc-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0fdc-121">JSON Representation</span></span>
<span data-ttu-id="b0fdc-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0fdc-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```





