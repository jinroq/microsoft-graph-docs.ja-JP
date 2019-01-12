---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513a6c545fedc73add4e710ed784ef223d1f8539
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976353"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="966d4-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="966d4-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="966d4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="966d4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="966d4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="966d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="966d4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="966d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="966d4-107">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="966d4-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="966d4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="966d4-108">Members</span></span>
|<span data-ttu-id="966d4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="966d4-109">Member</span></span>|<span data-ttu-id="966d4-110">値</span><span class="sxs-lookup"><span data-stu-id="966d4-110">Value</span></span>|<span data-ttu-id="966d4-111">説明</span><span class="sxs-lookup"><span data-stu-id="966d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="966d4-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="966d4-112">deviceDefault</span></span>|<span data-ttu-id="966d4-113">0</span><span class="sxs-lookup"><span data-stu-id="966d4-113">0</span></span>|<span data-ttu-id="966d4-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="966d4-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="966d4-115">none</span><span class="sxs-lookup"><span data-stu-id="966d4-115">none</span></span>|<span data-ttu-id="966d4-116">1</span><span class="sxs-lookup"><span data-stu-id="966d4-116">1</span></span>|<span data-ttu-id="966d4-117">事前共有キーはエンコードされません。</span><span class="sxs-lookup"><span data-stu-id="966d4-117">Preshared key is not encoded.</span></span> <span data-ttu-id="966d4-118">ワイド文字形式で保存される代わりに、</span><span class="sxs-lookup"><span data-stu-id="966d4-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="966d4-119">utF8</span><span class="sxs-lookup"><span data-stu-id="966d4-119">utF8</span></span>|<span data-ttu-id="966d4-120">2</span><span class="sxs-lookup"><span data-stu-id="966d4-120">2</span></span>|<span data-ttu-id="966d4-121">UTF-8 を使用して事前共有キーをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="966d4-121">Encode the preshared key using UTF-8</span></span>|





