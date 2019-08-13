---
title: win32LobAppReturnCode リソースの種類
description: Win32 アプリのリターンコードプロパティを格納します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84b2798956ec2b88b4c4dea212fb614f26ff1eff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335488"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="0ef69-103">win32LobAppReturnCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ef69-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="0ef69-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ef69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ef69-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ef69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ef69-106">Win32 アプリのリターンコードプロパティを格納します。</span><span class="sxs-lookup"><span data-stu-id="0ef69-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="0ef69-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ef69-107">Properties</span></span>
|<span data-ttu-id="0ef69-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ef69-108">Property</span></span>|<span data-ttu-id="0ef69-109">型</span><span class="sxs-lookup"><span data-stu-id="0ef69-109">Type</span></span>|<span data-ttu-id="0ef69-110">説明</span><span class="sxs-lookup"><span data-stu-id="0ef69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ef69-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="0ef69-111">returnCode</span></span>|<span data-ttu-id="0ef69-112">Int32</span><span class="sxs-lookup"><span data-stu-id="0ef69-112">Int32</span></span>|<span data-ttu-id="0ef69-113">コードを返します。</span><span class="sxs-lookup"><span data-stu-id="0ef69-113">Return code.</span></span>|
|<span data-ttu-id="0ef69-114">type</span><span class="sxs-lookup"><span data-stu-id="0ef69-114">type</span></span>|[<span data-ttu-id="0ef69-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="0ef69-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="0ef69-116">戻り値のコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="0ef69-116">The type of return code.</span></span> <span data-ttu-id="0ef69-117">可能な値は、`failed`、`success`、`softReboot`、`hardReboot`、`retry` です。</span><span class="sxs-lookup"><span data-stu-id="0ef69-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ef69-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ef69-118">Relationships</span></span>
<span data-ttu-id="0ef69-119">なし</span><span class="sxs-lookup"><span data-stu-id="0ef69-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ef69-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ef69-120">JSON Representation</span></span>
<span data-ttu-id="0ef69-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ef69-121">Here is a JSON representation of the resource.</span></span>
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



