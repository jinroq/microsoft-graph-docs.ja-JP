---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b72553fcc9cc55c3455a64eee5d6a8f75be6621
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831438"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="aeb4f-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aeb4f-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="aeb4f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aeb4f-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeb4f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aeb4f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aeb4f-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aeb4f-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aeb4f-108">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="aeb4f-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="aeb4f-109">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="aeb4f-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="aeb4f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aeb4f-110">Properties</span></span>
|<span data-ttu-id="aeb4f-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aeb4f-111">Property</span></span>|<span data-ttu-id="aeb4f-112">種類</span><span class="sxs-lookup"><span data-stu-id="aeb4f-112">Type</span></span>|<span data-ttu-id="aeb4f-113">説明</span><span class="sxs-lookup"><span data-stu-id="aeb4f-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="aeb4f-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aeb4f-114">Relationships</span></span>
<span data-ttu-id="aeb4f-115">なし</span><span class="sxs-lookup"><span data-stu-id="aeb4f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aeb4f-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aeb4f-116">JSON Representation</span></span>
<span data-ttu-id="aeb4f-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aeb4f-117">Here is a JSON representation of the resource.</span></span>
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





