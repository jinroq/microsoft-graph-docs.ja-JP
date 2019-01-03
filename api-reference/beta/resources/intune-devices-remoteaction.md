---
title: remoteAction 列挙型
description: リモート操作 Intune をサポートしています。
author: tfitzmac
ms.openlocfilehash: 7b301757ec5bb8c9c9a0336cbc83d6a458579916
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362560"
---
# <a name="remoteaction-enum-type"></a><span data-ttu-id="98c8c-103">remoteAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="98c8c-103">remoteAction enum type</span></span>

> <span data-ttu-id="98c8c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98c8c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98c8c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98c8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98c8c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="98c8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98c8c-107">リモート操作 Intune をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="98c8c-107">Remote actions Intune supports.</span></span>
## <a name="members"></a><span data-ttu-id="98c8c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="98c8c-108">Members</span></span>
|<span data-ttu-id="98c8c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="98c8c-109">Member</span></span>|<span data-ttu-id="98c8c-110">値</span><span class="sxs-lookup"><span data-stu-id="98c8c-110">Value</span></span>|<span data-ttu-id="98c8c-111">説明</span><span class="sxs-lookup"><span data-stu-id="98c8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98c8c-112">不明</span><span class="sxs-lookup"><span data-stu-id="98c8c-112">unknown</span></span>|<span data-ttu-id="98c8c-113">0</span><span class="sxs-lookup"><span data-stu-id="98c8c-113">0</span></span>|<span data-ttu-id="98c8c-114">ユーザーは、不明なアクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-114">User initiates an unknown action.</span></span>|
|<span data-ttu-id="98c8c-115">factoryReset</span><span class="sxs-lookup"><span data-stu-id="98c8c-115">factoryReset</span></span>|<span data-ttu-id="98c8c-116">1</span><span class="sxs-lookup"><span data-stu-id="98c8c-116">1</span></span>|<span data-ttu-id="98c8c-117">工場出荷時の動作を開始するユーザーは、デバイスをリセットします。</span><span class="sxs-lookup"><span data-stu-id="98c8c-117">User initiates an action to factory reset a device.</span></span> |
|<span data-ttu-id="98c8c-118">removeCompanyData</span><span class="sxs-lookup"><span data-stu-id="98c8c-118">removeCompanyData</span></span>|<span data-ttu-id="98c8c-119">2</span><span class="sxs-lookup"><span data-stu-id="98c8c-119">2</span></span>|<span data-ttu-id="98c8c-120">ユーザーは、デバイスから企業データを削除するアクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-120">User initiates an action to remove company data from a device.</span></span> |
|<span data-ttu-id="98c8c-121">resetPasscode</span><span class="sxs-lookup"><span data-stu-id="98c8c-121">resetPasscode</span></span>|<span data-ttu-id="98c8c-122">3</span><span class="sxs-lookup"><span data-stu-id="98c8c-122">3</span></span>|<span data-ttu-id="98c8c-123">ユーザーが、iOS デバイスのパスコードを削除するか、アプリのパスコードをリセットする操作を開始すると Windows のデバイスです。</span><span class="sxs-lookup"><span data-stu-id="98c8c-123">User initiates an action to remove the passcode of an iOS device, or reset the passcode of Android / Windows device.</span></span> |
|<span data-ttu-id="98c8c-124">remoteLock</span><span class="sxs-lookup"><span data-stu-id="98c8c-124">remoteLock</span></span>|<span data-ttu-id="98c8c-125">4</span><span class="sxs-lookup"><span data-stu-id="98c8c-125">4</span></span>|<span data-ttu-id="98c8c-126">ユーザーは、デバイスをリモート ロック操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-126">User initiates an action to remote lock a device.</span></span>|
|<span data-ttu-id="98c8c-127">enableLostMode</span><span class="sxs-lookup"><span data-stu-id="98c8c-127">enableLostMode</span></span>|<span data-ttu-id="98c8c-128">5</span><span class="sxs-lookup"><span data-stu-id="98c8c-128">5</span></span>|<span data-ttu-id="98c8c-129">ユーザーは、コールを管理する iOS デバイス上で失われたモードを有効にする操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-129">User initiates an action to enable lost mode on a supervised iOS device.</span></span>|
|<span data-ttu-id="98c8c-130">disableLostMode</span><span class="sxs-lookup"><span data-stu-id="98c8c-130">disableLostMode</span></span>|<span data-ttu-id="98c8c-131">6</span><span class="sxs-lookup"><span data-stu-id="98c8c-131">6</span></span>|<span data-ttu-id="98c8c-132">ユーザーは、コールを管理する iOS デバイス上で失われたモードを無効にする操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-132">User initiates an action to disable lost mode on a supervised iOS device.</span></span>|
|<span data-ttu-id="98c8c-133">locateDevice</span><span class="sxs-lookup"><span data-stu-id="98c8c-133">locateDevice</span></span>|<span data-ttu-id="98c8c-134">7</span><span class="sxs-lookup"><span data-stu-id="98c8c-134">7</span></span>|<span data-ttu-id="98c8c-135">ユーザーは、コールを管理する iOS デバイスを検索する操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-135">User initiates an action to locate a supervised iOS device.</span></span>|
|<span data-ttu-id="98c8c-136">rebootNow</span><span class="sxs-lookup"><span data-stu-id="98c8c-136">rebootNow</span></span>|<span data-ttu-id="98c8c-137">8</span><span class="sxs-lookup"><span data-stu-id="98c8c-137">8</span></span>|<span data-ttu-id="98c8c-138">ユーザーは、Windows のデバイスを再起動する操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-138">User initiates an action to reboot a Windows device.</span></span>|
|<span data-ttu-id="98c8c-139">recoverPasscode</span><span class="sxs-lookup"><span data-stu-id="98c8c-139">recoverPasscode</span></span>|<span data-ttu-id="98c8c-140">9</span><span class="sxs-lookup"><span data-stu-id="98c8c-140">9</span></span>|<span data-ttu-id="98c8c-141">ユーザーは、windows の電話デバイスでの作業の passport の pin をリセットするのにはアクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-141">User initiates an action to reset the pin for passport for work on windows phone device.</span></span>|
|<span data-ttu-id="98c8c-142">cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="98c8c-142">cleanWindowsDevice</span></span>|<span data-ttu-id="98c8c-143">10</span><span class="sxs-lookup"><span data-stu-id="98c8c-143">10</span></span>|<span data-ttu-id="98c8c-144">ユーザーは、windows のデバイスをクリーンアップする処理を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-144">User initiates an action to clean up windows device.</span></span>|
|<span data-ttu-id="98c8c-145">logoutSharedAppleDeviceActiveUser</span><span class="sxs-lookup"><span data-stu-id="98c8c-145">logoutSharedAppleDeviceActiveUser</span></span>|<span data-ttu-id="98c8c-146">11</span><span class="sxs-lookup"><span data-stu-id="98c8c-146">11</span></span>|<span data-ttu-id="98c8c-147">ユーザーは、共有の apple デバイス上の現在のユーザーをログアウトする操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-147">User initiates an action to log out current user on shared apple device.</span></span>|
|<span data-ttu-id="98c8c-148">quickScan</span><span class="sxs-lookup"><span data-stu-id="98c8c-148">quickScan</span></span>|<span data-ttu-id="98c8c-149">12</span><span class="sxs-lookup"><span data-stu-id="98c8c-149">12</span></span>|<span data-ttu-id="98c8c-150">ユーザーは、デバイス上のクイック スキャンを実行するアクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-150">User initiates an action to run quick scan on device.</span></span>|
|<span data-ttu-id="98c8c-151">fullScan</span><span class="sxs-lookup"><span data-stu-id="98c8c-151">fullScan</span></span>|<span data-ttu-id="98c8c-152">13</span><span class="sxs-lookup"><span data-stu-id="98c8c-152">13</span></span>|<span data-ttu-id="98c8c-153">ユーザーは、デバイスの完全なスキャンを実行するアクションを開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-153">User initiates an action to run full scan on device.</span></span>|
|<span data-ttu-id="98c8c-154">windowsDefenderUpdateSignatures</span><span class="sxs-lookup"><span data-stu-id="98c8c-154">windowsDefenderUpdateSignatures</span></span>|<span data-ttu-id="98c8c-155">14</span><span class="sxs-lookup"><span data-stu-id="98c8c-155">14</span></span>|<span data-ttu-id="98c8c-156">ユーザーは、デバイス上のマルウェアの署名を更新する操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-156">User initiates an action to update malware signatures on device.</span></span>|
|<span data-ttu-id="98c8c-157">factoryResetKeepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="98c8c-157">factoryResetKeepEnrollmentData</span></span>|<span data-ttu-id="98c8c-158">15</span><span class="sxs-lookup"><span data-stu-id="98c8c-158">15</span></span>|<span data-ttu-id="98c8c-159">ユーザーは、登録データを保持することで、デバイスを操作リモート ワイプを開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-159">User initiates an action remote wipe device with keeping enrollment data.</span></span>|
|<span data-ttu-id="98c8c-160">updateDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="98c8c-160">updateDeviceAccount</span></span>|<span data-ttu-id="98c8c-161">16</span><span class="sxs-lookup"><span data-stu-id="98c8c-161">16</span></span>|<span data-ttu-id="98c8c-162">ユーザーは、デバイス上のアカウントを更新する操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-162">User initiates an action to update account on device.</span></span>|
|<span data-ttu-id="98c8c-163">automaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="98c8c-163">automaticRedeployment</span></span>|<span data-ttu-id="98c8c-164">17</span><span class="sxs-lookup"><span data-stu-id="98c8c-164">17</span></span>|<span data-ttu-id="98c8c-165">ユーザーが automatice デバイスを再配置する操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-165">User initiates an action to automatice redeploy the device</span></span>|
|<span data-ttu-id="98c8c-166">シャット ダウン</span><span class="sxs-lookup"><span data-stu-id="98c8c-166">shutDown</span></span>|<span data-ttu-id="98c8c-167">18</span><span class="sxs-lookup"><span data-stu-id="98c8c-167">18</span></span>|<span data-ttu-id="98c8c-168">ユーザーは、デバイスをシャット ダウンする操作を開始します。</span><span class="sxs-lookup"><span data-stu-id="98c8c-168">User initiates an action to shut down the device.</span></span>|




