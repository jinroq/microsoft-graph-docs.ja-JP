---
title: automaticUpdateMode 列挙型
description: 自動更新モードを使用可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a31c50b5d16f4b9be8db4f95f2bbd9bd0ca123e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987861"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="178c6-103">automaticUpdateMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="178c6-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="178c6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="178c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="178c6-105">自動更新モードを使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="178c6-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="178c6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="178c6-106">Members</span></span>
|<span data-ttu-id="178c6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="178c6-107">Member</span></span>|<span data-ttu-id="178c6-108">値</span><span class="sxs-lookup"><span data-stu-id="178c6-108">Value</span></span>|<span data-ttu-id="178c6-109">説明</span><span class="sxs-lookup"><span data-stu-id="178c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="178c6-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="178c6-110">userDefined</span></span>|<span data-ttu-id="178c6-111">0</span><span class="sxs-lookup"><span data-stu-id="178c6-111">0</span></span>|<span data-ttu-id="178c6-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="178c6-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="178c6-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="178c6-113">notifyDownload</span></span>|<span data-ttu-id="178c6-114">1</span><span class="sxs-lookup"><span data-stu-id="178c6-114">1</span></span>|<span data-ttu-id="178c6-115">ダウンロード時に通知します。</span><span class="sxs-lookup"><span data-stu-id="178c6-115">Notify on download.</span></span>|
|<span data-ttu-id="178c6-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="178c6-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="178c6-117">2</span><span class="sxs-lookup"><span data-stu-id="178c6-117">2</span></span>|<span data-ttu-id="178c6-118">メンテナンス時に自動インストールします。</span><span class="sxs-lookup"><span data-stu-id="178c6-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="178c6-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="178c6-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="178c6-120">3</span><span class="sxs-lookup"><span data-stu-id="178c6-120">3</span></span>|<span data-ttu-id="178c6-121">自動インストールおよびメンテナンス時に再起動します。</span><span class="sxs-lookup"><span data-stu-id="178c6-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="178c6-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="178c6-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="178c6-123">4</span><span class="sxs-lookup"><span data-stu-id="178c6-123">4</span></span>|<span data-ttu-id="178c6-124">自動インストールし、スケジュールされた時刻に再起動します。</span><span class="sxs-lookup"><span data-stu-id="178c6-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="178c6-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="178c6-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="178c6-126">5</span><span class="sxs-lookup"><span data-stu-id="178c6-126">5</span></span>|<span data-ttu-id="178c6-127">自動インストールし、エンドユーザーの制御に再起動します</span><span class="sxs-lookup"><span data-stu-id="178c6-127">Auto-install and restart without end-user control</span></span>|



