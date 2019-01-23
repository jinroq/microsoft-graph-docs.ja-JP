---
title: androidPermissionAction リソースの種類
description: Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425632"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="a0ab1-103">androidPermissionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0ab1-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="a0ab1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0ab1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0ab1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0ab1-107">Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="a0ab1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0ab1-108">Properties</span></span>
|<span data-ttu-id="a0ab1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0ab1-109">Property</span></span>|<span data-ttu-id="a0ab1-110">型</span><span class="sxs-lookup"><span data-stu-id="a0ab1-110">Type</span></span>|<span data-ttu-id="a0ab1-111">説明</span><span class="sxs-lookup"><span data-stu-id="a0ab1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0ab1-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a0ab1-112">permission</span></span>|<span data-ttu-id="a0ab1-113">String</span><span class="sxs-lookup"><span data-stu-id="a0ab1-113">String</span></span>|<span data-ttu-id="a0ab1-114">Android のアクセス許可の文字列、公式の Android のドキュメントで定義されています。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="a0ab1-115">'Android.permission.READ_CONTACTS' の使用例です。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="a0ab1-116">action</span><span class="sxs-lookup"><span data-stu-id="a0ab1-116">action</span></span>|[<span data-ttu-id="a0ab1-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="a0ab1-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="a0ab1-118">Android 権限操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-118">Type of Android permission action.</span></span> <span data-ttu-id="a0ab1-119">可能な値は、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0ab1-120">関係</span><span class="sxs-lookup"><span data-stu-id="a0ab1-120">Relationships</span></span>
<span data-ttu-id="a0ab1-121">なし</span><span class="sxs-lookup"><span data-stu-id="a0ab1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0ab1-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0ab1-122">JSON Representation</span></span>
<span data-ttu-id="a0ab1-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0ab1-123">Here is a JSON representation of the resource.</span></span>
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




