---
title: androidpermissionaction リソースの種類
description: android アプリのアクセス許可と android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fec33b2600e88e6a4dfae644c335d9652c20abe0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552353"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="c155c-103">androidpermissionaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c155c-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="c155c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c155c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c155c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c155c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c155c-106">android アプリのアクセス許可と android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。</span><span class="sxs-lookup"><span data-stu-id="c155c-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="c155c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c155c-107">Properties</span></span>
|<span data-ttu-id="c155c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c155c-108">Property</span></span>|<span data-ttu-id="c155c-109">型</span><span class="sxs-lookup"><span data-stu-id="c155c-109">Type</span></span>|<span data-ttu-id="c155c-110">説明</span><span class="sxs-lookup"><span data-stu-id="c155c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c155c-111">権</span><span class="sxs-lookup"><span data-stu-id="c155c-111">permission</span></span>|<span data-ttu-id="c155c-112">String</span><span class="sxs-lookup"><span data-stu-id="c155c-112">String</span></span>|<span data-ttu-id="c155c-113">android のアクセス許可文字列。公式の android ドキュメントで定義されています。</span><span class="sxs-lookup"><span data-stu-id="c155c-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="c155c-114">例 ' READ_CONTACTS '。</span><span class="sxs-lookup"><span data-stu-id="c155c-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="c155c-115">action</span><span class="sxs-lookup"><span data-stu-id="c155c-115">action</span></span>|[<span data-ttu-id="c155c-116">androidpermissionactiontype</span><span class="sxs-lookup"><span data-stu-id="c155c-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="c155c-117">Android のアクセス許可アクションの種類。</span><span class="sxs-lookup"><span data-stu-id="c155c-117">Type of Android permission action.</span></span> <span data-ttu-id="c155c-118">可能な値は、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="c155c-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c155c-119">関係</span><span class="sxs-lookup"><span data-stu-id="c155c-119">Relationships</span></span>
<span data-ttu-id="c155c-120">なし</span><span class="sxs-lookup"><span data-stu-id="c155c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c155c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c155c-121">JSON Representation</span></span>
<span data-ttu-id="c155c-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c155c-122">Here is a JSON representation of the resource.</span></span>
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





