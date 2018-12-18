---
title: Intune を使用して会社所有のデバイスを登録する
description: " (BYOD) のシナリオです。"
author: tfitzmac
ms.openlocfilehash: f3103d2098053a75839b297eb4ef0a656d6d53a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334322"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="3071b-103">Intune を使用して会社所有のデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="3071b-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="3071b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3071b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="3071b-105">組織所有または会社所有のデバイスを登録して、デバイスの種類、デバイスの購入方法、組織のニーズに応じて、さまざまな方法で Intune で管理することができます。</span><span class="sxs-lookup"><span data-stu-id="3071b-105">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="3071b-106">また、ポータル サイト アプリをインストールして、会社所有のデバイスの登録と管理を、"Bring Your Own Device" (BYOD) のようなシナリオで行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="3071b-106">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="3071b-107">次の Graph リソースを使用して、Intune での会社所有のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="3071b-107">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="3071b-108">インポートされた windows の自動操縦装置のデバイス id</span><span class="sxs-lookup"><span data-stu-id="3071b-108">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="3071b-109">インポートされた windows 自動操縦装置のデバイス id のインポート状態</span><span class="sxs-lookup"><span data-stu-id="3071b-109">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="3071b-110">インポートされた windows 自動操縦装置のアイデンティティの状態</span><span class="sxs-lookup"><span data-stu-id="3071b-110">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="3071b-111">インポートされた windows 自動操縦装置のデバイス識別情報のアップロード</span><span class="sxs-lookup"><span data-stu-id="3071b-111">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="3071b-112">インポートされた windows 自動操縦装置のデバイス id アップロード状態</span><span class="sxs-lookup"><span data-stu-id="3071b-112">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
