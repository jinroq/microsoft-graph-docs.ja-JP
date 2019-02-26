---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d9858eb8277b804d5fb90acd8efc9174c7c8bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161972"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="9e540-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e540-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="9e540-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e540-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e540-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e540-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e540-107">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="9e540-107">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="9e540-108">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="9e540-108">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="9e540-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e540-109">Properties</span></span>
|<span data-ttu-id="9e540-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e540-110">Property</span></span>|<span data-ttu-id="9e540-111">型</span><span class="sxs-lookup"><span data-stu-id="9e540-111">Type</span></span>|<span data-ttu-id="9e540-112">説明</span><span class="sxs-lookup"><span data-stu-id="9e540-112">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="9e540-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9e540-113">Relationships</span></span>
<span data-ttu-id="9e540-114">なし</span><span class="sxs-lookup"><span data-stu-id="9e540-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e540-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e540-115">JSON Representation</span></span>
<span data-ttu-id="9e540-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9e540-116">Here is a JSON representation of the resource.</span></span>
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




