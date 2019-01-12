---
title: windowsStartMenuAppListVisibilityType 列挙型
description: '[スタート] メニューの [アプリケーション] ボックスの一覧の可視性のタイプです。'
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4b2e07126ab6f65af26a8145c04acbab526ab8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932589"
---
# <a name="windowsstartmenuapplistvisibilitytype-enum-type"></a><span data-ttu-id="c365d-103">windowsStartMenuAppListVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c365d-103">windowsStartMenuAppListVisibilityType enum type</span></span>

> <span data-ttu-id="c365d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c365d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c365d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c365d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c365d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c365d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c365d-107">[スタート] メニューの [アプリケーション] ボックスの一覧の可視性のタイプです。</span><span class="sxs-lookup"><span data-stu-id="c365d-107">Type of start menu app list visibility.</span></span>
## <a name="members"></a><span data-ttu-id="c365d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c365d-108">Members</span></span>
|<span data-ttu-id="c365d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c365d-109">Member</span></span>|<span data-ttu-id="c365d-110">値</span><span class="sxs-lookup"><span data-stu-id="c365d-110">Value</span></span>|<span data-ttu-id="c365d-111">説明</span><span class="sxs-lookup"><span data-stu-id="c365d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c365d-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="c365d-112">userDefined</span></span>|<span data-ttu-id="c365d-113">0</span><span class="sxs-lookup"><span data-stu-id="c365d-113">0</span></span>|<span data-ttu-id="c365d-114">ユーザーが定義します。</span><span class="sxs-lookup"><span data-stu-id="c365d-114">User defined.</span></span> <span data-ttu-id="c365d-115">既定値です。</span><span class="sxs-lookup"><span data-stu-id="c365d-115">Default value.</span></span>|
|<span data-ttu-id="c365d-116">折りたたみ</span><span class="sxs-lookup"><span data-stu-id="c365d-116">collapse</span></span>|<span data-ttu-id="c365d-117">1</span><span class="sxs-lookup"><span data-stu-id="c365d-117">1</span></span>|<span data-ttu-id="c365d-118">[スタート] メニューの [アプリケーション] ボックスの一覧を折りたたみます。</span><span class="sxs-lookup"><span data-stu-id="c365d-118">Collapse the app list on the start menu.</span></span>|
|<span data-ttu-id="c365d-119">remove</span><span class="sxs-lookup"><span data-stu-id="c365d-119">remove</span></span>|<span data-ttu-id="c365d-120">2</span><span class="sxs-lookup"><span data-stu-id="c365d-120">2</span></span>|<span data-ttu-id="c365d-121">[スタート] メニューから、[アプリケーション] ボックスの一覧を削除します。</span><span class="sxs-lookup"><span data-stu-id="c365d-121">Removes the app list entirely from the start menu.</span></span>|
|<span data-ttu-id="c365d-122">disableSettingsApp</span><span class="sxs-lookup"><span data-stu-id="c365d-122">disableSettingsApp</span></span>|<span data-ttu-id="c365d-123">4</span><span class="sxs-lookup"><span data-stu-id="c365d-123">4</span></span>|<span data-ttu-id="c365d-124">設定アプリで対応する切り替え (縮小または削除する) を無効にします。</span><span class="sxs-lookup"><span data-stu-id="c365d-124">Disables the corresponding toggle (Collapse or Remove) in the Settings app.</span></span>|





