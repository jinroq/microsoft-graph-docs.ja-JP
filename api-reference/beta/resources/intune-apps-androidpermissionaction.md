---
title: androidPermissionAction リソースの種類
description: Android アプリのアクセス許可と Android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d2aa07ae9064a6e7d04ea7e2f0dc07e06cfb627
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366890"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="b62f6-103">androidPermissionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b62f6-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="b62f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b62f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b62f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b62f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b62f6-106">Android アプリのアクセス許可と Android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。</span><span class="sxs-lookup"><span data-stu-id="b62f6-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="b62f6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b62f6-107">Properties</span></span>
|<span data-ttu-id="b62f6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b62f6-108">Property</span></span>|<span data-ttu-id="b62f6-109">型</span><span class="sxs-lookup"><span data-stu-id="b62f6-109">Type</span></span>|<span data-ttu-id="b62f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="b62f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b62f6-111">権</span><span class="sxs-lookup"><span data-stu-id="b62f6-111">permission</span></span>|<span data-ttu-id="b62f6-112">String</span><span class="sxs-lookup"><span data-stu-id="b62f6-112">String</span></span>|<span data-ttu-id="b62f6-113">Android のアクセス許可文字列。公式の Android ドキュメントで定義されています。</span><span class="sxs-lookup"><span data-stu-id="b62f6-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="b62f6-114">例 ' READ_CONTACTS '。</span><span class="sxs-lookup"><span data-stu-id="b62f6-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="b62f6-115">action</span><span class="sxs-lookup"><span data-stu-id="b62f6-115">action</span></span>|[<span data-ttu-id="b62f6-116">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="b62f6-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="b62f6-117">Android のアクセス許可アクションの種類。</span><span class="sxs-lookup"><span data-stu-id="b62f6-117">Type of Android permission action.</span></span> <span data-ttu-id="b62f6-118">可能な値は、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="b62f6-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b62f6-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b62f6-119">Relationships</span></span>
<span data-ttu-id="b62f6-120">なし</span><span class="sxs-lookup"><span data-stu-id="b62f6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b62f6-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b62f6-121">JSON Representation</span></span>
<span data-ttu-id="b62f6-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b62f6-122">Here is a JSON representation of the resource.</span></span>
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



