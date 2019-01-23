---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2cc8a0fee08826fef7d560a18f730bd7d58a2f6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417232"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="2cad2-103">educationSynchronizationOAuth1ConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="2cad2-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="2cad2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2cad2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cad2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cad2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2cad2-106">データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="2cad2-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="2cad2-107">[Microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="2cad2-107">Derived from [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2cad2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cad2-108">Properties</span></span>

<span data-ttu-id="2cad2-109">この型では、追加のプロパティは公開されません。</span><span class="sxs-lookup"><span data-stu-id="2cad2-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cad2-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cad2-110">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
