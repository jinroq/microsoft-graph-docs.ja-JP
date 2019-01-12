---
title: win32LobAppReturnCode リソースの種類
description: Win32 アプリケーションのプロパティ戻り値のコードにはが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0728ee3c029331b37369172373ef1400dde37991
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927864"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="55a27-103">win32LobAppReturnCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55a27-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="55a27-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55a27-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55a27-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55a27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55a27-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="55a27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55a27-107">Win32 アプリケーションのプロパティ戻り値のコードにはが含まれています</span><span class="sxs-lookup"><span data-stu-id="55a27-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="55a27-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55a27-108">Properties</span></span>
|<span data-ttu-id="55a27-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55a27-109">Property</span></span>|<span data-ttu-id="55a27-110">種類</span><span class="sxs-lookup"><span data-stu-id="55a27-110">Type</span></span>|<span data-ttu-id="55a27-111">説明</span><span class="sxs-lookup"><span data-stu-id="55a27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55a27-112">リターン コード</span><span class="sxs-lookup"><span data-stu-id="55a27-112">returnCode</span></span>|<span data-ttu-id="55a27-113">Int32</span><span class="sxs-lookup"><span data-stu-id="55a27-113">Int32</span></span>|<span data-ttu-id="55a27-114">コードを返します。</span><span class="sxs-lookup"><span data-stu-id="55a27-114">Return code.</span></span>|
|<span data-ttu-id="55a27-115">type</span><span class="sxs-lookup"><span data-stu-id="55a27-115">type</span></span>|[<span data-ttu-id="55a27-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="55a27-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="55a27-117">コードの戻り値の型。</span><span class="sxs-lookup"><span data-stu-id="55a27-117">The type of return code.</span></span> <span data-ttu-id="55a27-118">可能な値は、`failed`、`success`、`softReboot`、`hardReboot`、`retry` です。</span><span class="sxs-lookup"><span data-stu-id="55a27-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55a27-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55a27-119">Relationships</span></span>
<span data-ttu-id="55a27-120">なし</span><span class="sxs-lookup"><span data-stu-id="55a27-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55a27-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55a27-121">JSON Representation</span></span>
<span data-ttu-id="55a27-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55a27-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```





