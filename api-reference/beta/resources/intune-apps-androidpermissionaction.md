---
title: androidPermissionAction リソースの種類
description: Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: daf72bbc5f8d1e32480adeda72c3f759255f54db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860537"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="ff0ef-103">androidPermissionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff0ef-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="ff0ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff0ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff0ef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff0ef-107">Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="ff0ef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff0ef-108">Properties</span></span>
|<span data-ttu-id="ff0ef-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff0ef-109">Property</span></span>|<span data-ttu-id="ff0ef-110">種類</span><span class="sxs-lookup"><span data-stu-id="ff0ef-110">Type</span></span>|<span data-ttu-id="ff0ef-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff0ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0ef-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff0ef-112">permission</span></span>|<span data-ttu-id="ff0ef-113">String</span><span class="sxs-lookup"><span data-stu-id="ff0ef-113">String</span></span>|<span data-ttu-id="ff0ef-114">Android のアクセス許可の文字列、公式の Android のドキュメントで定義されています。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="ff0ef-115">'Android.permission.READ_CONTACTS' の使用例です。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="ff0ef-116">action</span><span class="sxs-lookup"><span data-stu-id="ff0ef-116">action</span></span>|[<span data-ttu-id="ff0ef-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="ff0ef-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="ff0ef-118">Android 権限操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-118">Type of Android permission action.</span></span> <span data-ttu-id="ff0ef-119">可能な値は、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff0ef-120">関係</span><span class="sxs-lookup"><span data-stu-id="ff0ef-120">Relationships</span></span>
<span data-ttu-id="ff0ef-121">なし</span><span class="sxs-lookup"><span data-stu-id="ff0ef-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff0ef-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff0ef-122">JSON Representation</span></span>
<span data-ttu-id="ff0ef-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff0ef-123">Here is a JSON representation of the resource.</span></span>
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





