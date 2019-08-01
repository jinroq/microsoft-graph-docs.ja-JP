---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a563d030a12480c6151a76cf2d58f743783bb378
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031543"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="7c6c4-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7c6c4-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="7c6c4-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c6c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c6c4-105">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="7c6c4-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="7c6c4-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="7c6c4-106">Members</span></span>
|<span data-ttu-id="7c6c4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7c6c4-107">Member</span></span>|<span data-ttu-id="7c6c4-108">値</span><span class="sxs-lookup"><span data-stu-id="7c6c4-108">Value</span></span>|<span data-ttu-id="7c6c4-109">説明</span><span class="sxs-lookup"><span data-stu-id="7c6c4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c6c4-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7c6c4-110">deviceDefault</span></span>|<span data-ttu-id="7c6c4-111">.0</span><span class="sxs-lookup"><span data-stu-id="7c6c4-111">0</span></span>|<span data-ttu-id="7c6c4-112">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="7c6c4-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7c6c4-113">none</span><span class="sxs-lookup"><span data-stu-id="7c6c4-113">none</span></span>|<span data-ttu-id="7c6c4-114">1-d</span><span class="sxs-lookup"><span data-stu-id="7c6c4-114">1</span></span>|<span data-ttu-id="7c6c4-115">事前共有キーはエンコードされていません。</span><span class="sxs-lookup"><span data-stu-id="7c6c4-115">Preshared key is not encoded.</span></span> <span data-ttu-id="7c6c4-116">代わりに、ワイド文字形式で保存されます。</span><span class="sxs-lookup"><span data-stu-id="7c6c4-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="7c6c4-117">utF8</span><span class="sxs-lookup"><span data-stu-id="7c6c4-117">utF8</span></span>|<span data-ttu-id="7c6c4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7c6c4-118">2</span></span>|<span data-ttu-id="7c6c4-119">UTF-8 を使用して事前共有キーをエンコードする</span><span class="sxs-lookup"><span data-stu-id="7c6c4-119">Encode the preshared key using UTF-8</span></span>|



