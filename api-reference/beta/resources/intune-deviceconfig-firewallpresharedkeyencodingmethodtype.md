---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 577925f141c6dd94b493664d3617df939d19c5c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410953"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="d1fe9-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d1fe9-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="d1fe9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1fe9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1fe9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1fe9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1fe9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1fe9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1fe9-107">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d1fe9-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="d1fe9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1fe9-108">Members</span></span>
|<span data-ttu-id="d1fe9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1fe9-109">Member</span></span>|<span data-ttu-id="d1fe9-110">値</span><span class="sxs-lookup"><span data-stu-id="d1fe9-110">Value</span></span>|<span data-ttu-id="d1fe9-111">説明</span><span class="sxs-lookup"><span data-stu-id="d1fe9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1fe9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d1fe9-112">deviceDefault</span></span>|<span data-ttu-id="d1fe9-113">0</span><span class="sxs-lookup"><span data-stu-id="d1fe9-113">0</span></span>|<span data-ttu-id="d1fe9-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="d1fe9-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d1fe9-115">none</span><span class="sxs-lookup"><span data-stu-id="d1fe9-115">none</span></span>|<span data-ttu-id="d1fe9-116">1</span><span class="sxs-lookup"><span data-stu-id="d1fe9-116">1</span></span>|<span data-ttu-id="d1fe9-117">事前共有キーはエンコードされません。</span><span class="sxs-lookup"><span data-stu-id="d1fe9-117">Preshared key is not encoded.</span></span> <span data-ttu-id="d1fe9-118">ワイド文字形式で保存される代わりに、</span><span class="sxs-lookup"><span data-stu-id="d1fe9-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="d1fe9-119">utF8</span><span class="sxs-lookup"><span data-stu-id="d1fe9-119">utF8</span></span>|<span data-ttu-id="d1fe9-120">2</span><span class="sxs-lookup"><span data-stu-id="d1fe9-120">2</span></span>|<span data-ttu-id="d1fe9-121">UTF-8 を使用して事前共有キーをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="d1fe9-121">Encode the preshared key using UTF-8</span></span>|




