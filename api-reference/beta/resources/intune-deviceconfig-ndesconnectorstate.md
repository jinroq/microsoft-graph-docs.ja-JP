---
title: ndesConnectorState 列挙型
description: Ndes コネクタの現在の状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3cb54495bffb065ddd56aae1edc063502b681e4c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990328"
---
# <a name="ndesconnectorstate-enum-type"></a><span data-ttu-id="83617-103">ndesConnectorState 列挙型</span><span class="sxs-lookup"><span data-stu-id="83617-103">ndesConnectorState enum type</span></span>

> <span data-ttu-id="83617-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83617-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83617-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83617-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83617-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83617-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83617-107">Ndes コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="83617-107">The current status of the Ndes Connector.</span></span>
## <a name="members"></a><span data-ttu-id="83617-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="83617-108">Members</span></span>
|<span data-ttu-id="83617-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="83617-109">Member</span></span>|<span data-ttu-id="83617-110">値</span><span class="sxs-lookup"><span data-stu-id="83617-110">Value</span></span>|<span data-ttu-id="83617-111">説明</span><span class="sxs-lookup"><span data-stu-id="83617-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83617-112">none</span><span class="sxs-lookup"><span data-stu-id="83617-112">none</span></span>|<span data-ttu-id="83617-113">0</span><span class="sxs-lookup"><span data-stu-id="83617-113">0</span></span>|<span data-ttu-id="83617-114">状態このコネクタはまだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="83617-114">State not available yet for this connector.</span></span>|
|<span data-ttu-id="83617-115">アクティブです</span><span class="sxs-lookup"><span data-stu-id="83617-115">active</span></span>|<span data-ttu-id="83617-116">1</span><span class="sxs-lookup"><span data-stu-id="83617-116">1</span></span>|<span data-ttu-id="83617-117">Ndes のコネクタが接続されている最近</span><span class="sxs-lookup"><span data-stu-id="83617-117">Ndes connector has connected recently</span></span>|
|<span data-ttu-id="83617-118">使用頻度の低い</span><span class="sxs-lookup"><span data-stu-id="83617-118">inactive</span></span>|<span data-ttu-id="83617-119">2</span><span class="sxs-lookup"><span data-stu-id="83617-119">2</span></span>|<span data-ttu-id="83617-120">Ndes のコネクタの最近のアクティビティはありません。</span><span class="sxs-lookup"><span data-stu-id="83617-120">No recent activity for the Ndes connector</span></span>|





