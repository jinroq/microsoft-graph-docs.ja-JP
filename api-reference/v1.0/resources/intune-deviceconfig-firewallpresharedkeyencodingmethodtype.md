---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: firewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62144ef2974da5a3d975c759bb8d2bd2be6032
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259550"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="d98d5-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d98d5-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="d98d5-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d98d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98d5-105">firewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d98d5-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="d98d5-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d98d5-106">Members</span></span>
|<span data-ttu-id="d98d5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d98d5-107">Member</span></span>|<span data-ttu-id="d98d5-108">値</span><span class="sxs-lookup"><span data-stu-id="d98d5-108">Value</span></span>|<span data-ttu-id="d98d5-109">説明</span><span class="sxs-lookup"><span data-stu-id="d98d5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98d5-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="d98d5-110">deviceDefault</span></span>|<span data-ttu-id="d98d5-111">.0</span><span class="sxs-lookup"><span data-stu-id="d98d5-111">0</span></span>|<span data-ttu-id="d98d5-112">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="d98d5-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d98d5-113">none</span><span class="sxs-lookup"><span data-stu-id="d98d5-113">none</span></span>|<span data-ttu-id="d98d5-114">1-d</span><span class="sxs-lookup"><span data-stu-id="d98d5-114">1</span></span>|<span data-ttu-id="d98d5-115">事前共有キーはエンコードされていません。</span><span class="sxs-lookup"><span data-stu-id="d98d5-115">Preshared key is not encoded.</span></span> <span data-ttu-id="d98d5-116">代わりに、ワイド文字形式で保存されます。</span><span class="sxs-lookup"><span data-stu-id="d98d5-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="d98d5-117">utF8</span><span class="sxs-lookup"><span data-stu-id="d98d5-117">utF8</span></span>|<span data-ttu-id="d98d5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d98d5-118">2</span></span>|<span data-ttu-id="d98d5-119">utf-8 を使用して事前共有キーをエンコードする</span><span class="sxs-lookup"><span data-stu-id="d98d5-119">Encode the preshared key using UTF-8</span></span>|



