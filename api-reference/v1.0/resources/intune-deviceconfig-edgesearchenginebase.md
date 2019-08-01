---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ddecca2341586d2f617ca75d7d0a89bcd8c182c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031620"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="232b7-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="232b7-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="232b7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="232b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="232b7-106">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="232b7-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="232b7-107">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="232b7-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="232b7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="232b7-108">Properties</span></span>
|<span data-ttu-id="232b7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="232b7-109">Property</span></span>|<span data-ttu-id="232b7-110">型</span><span class="sxs-lookup"><span data-stu-id="232b7-110">Type</span></span>|<span data-ttu-id="232b7-111">説明</span><span class="sxs-lookup"><span data-stu-id="232b7-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="232b7-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="232b7-112">Relationships</span></span>
<span data-ttu-id="232b7-113">なし</span><span class="sxs-lookup"><span data-stu-id="232b7-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="232b7-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="232b7-114">JSON Representation</span></span>
<span data-ttu-id="232b7-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="232b7-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```



