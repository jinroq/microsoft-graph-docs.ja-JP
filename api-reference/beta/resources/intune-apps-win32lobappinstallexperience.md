---
title: win32LobAppInstallExperience リソースの種類
description: Win32 アプリケーションのインストール環境のプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9eeadf7bc97f53278ef59fe06795bc7120d5bc2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986300"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="a0286-103">win32LobAppInstallExperience リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0286-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="a0286-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0286-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0286-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0286-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0286-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a0286-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0286-107">Win32 アプリケーションのインストール環境のプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="a0286-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="a0286-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0286-108">Properties</span></span>
|<span data-ttu-id="a0286-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0286-109">Property</span></span>|<span data-ttu-id="a0286-110">型</span><span class="sxs-lookup"><span data-stu-id="a0286-110">Type</span></span>|<span data-ttu-id="a0286-111">説明</span><span class="sxs-lookup"><span data-stu-id="a0286-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0286-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="a0286-112">runAsAccount</span></span>|[<span data-ttu-id="a0286-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="a0286-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="a0286-114">アプリケーションが実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="a0286-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="a0286-115">可能な値: `system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="a0286-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0286-116">関係</span><span class="sxs-lookup"><span data-stu-id="a0286-116">Relationships</span></span>
<span data-ttu-id="a0286-117">なし</span><span class="sxs-lookup"><span data-stu-id="a0286-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0286-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0286-118">JSON Representation</span></span>
<span data-ttu-id="a0286-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0286-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```





