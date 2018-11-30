---
title: androidPermissionAction リソースの種類
description: Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。
ms.openlocfilehash: e65f9b28169e231e34b5a7a46316821f77639233
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068507"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="4caf4-103">androidPermissionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4caf4-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="4caf4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4caf4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4caf4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4caf4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4caf4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4caf4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4caf4-107">Android アプリケーションのアクセス許可とアプリの操作の間のマッピングは、そのアクセス許可が要求されたときにかかります。</span><span class="sxs-lookup"><span data-stu-id="4caf4-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="4caf4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4caf4-108">Properties</span></span>
|<span data-ttu-id="4caf4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4caf4-109">Property</span></span>|<span data-ttu-id="4caf4-110">型</span><span class="sxs-lookup"><span data-stu-id="4caf4-110">Type</span></span>|<span data-ttu-id="4caf4-111">説明</span><span class="sxs-lookup"><span data-stu-id="4caf4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4caf4-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4caf4-112">permission</span></span>|<span data-ttu-id="4caf4-113">String</span><span class="sxs-lookup"><span data-stu-id="4caf4-113">String</span></span>|<span data-ttu-id="4caf4-114">Android のアクセス許可の文字列、公式の Android のドキュメントで定義されています。</span><span class="sxs-lookup"><span data-stu-id="4caf4-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="4caf4-115">'Android.permission.READ_CONTACTS' の使用例です。</span><span class="sxs-lookup"><span data-stu-id="4caf4-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="4caf4-116">action</span><span class="sxs-lookup"><span data-stu-id="4caf4-116">action</span></span>|[<span data-ttu-id="4caf4-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="4caf4-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="4caf4-118">Android 権限操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="4caf4-118">Type of Android permission action.</span></span> <span data-ttu-id="4caf4-119">可能な値は、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="4caf4-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4caf4-120">関係</span><span class="sxs-lookup"><span data-stu-id="4caf4-120">Relationships</span></span>
<span data-ttu-id="4caf4-121">なし</span><span class="sxs-lookup"><span data-stu-id="4caf4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4caf4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4caf4-122">JSON Representation</span></span>
<span data-ttu-id="4caf4-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4caf4-123">Here is a JSON representation of the resource.</span></span>
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





