---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
author: tfitzmac
ms.openlocfilehash: 1a9c1dc12226bf13764a155e804d379d20825103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344234"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="63b81-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63b81-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="63b81-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63b81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63b81-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63b81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63b81-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="63b81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63b81-107">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="63b81-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="63b81-108">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="63b81-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63b81-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63b81-109">Properties</span></span>
|<span data-ttu-id="63b81-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63b81-110">Property</span></span>|<span data-ttu-id="63b81-111">種類</span><span class="sxs-lookup"><span data-stu-id="63b81-111">Type</span></span>|<span data-ttu-id="63b81-112">説明</span><span class="sxs-lookup"><span data-stu-id="63b81-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b81-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="63b81-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="63b81-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="63b81-114">String</span></span>|<span data-ttu-id="63b81-115">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="63b81-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63b81-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="63b81-116">Relationships</span></span>
<span data-ttu-id="63b81-117">なし</span><span class="sxs-lookup"><span data-stu-id="63b81-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63b81-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63b81-118">JSON Representation</span></span>
<span data-ttu-id="63b81-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="63b81-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```





