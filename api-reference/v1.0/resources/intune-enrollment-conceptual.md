---
title: Intune を使用して会社所有のデバイスを登録する
description: " (BYOD) シナリオ。"
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: dc408612ed1ec0927076c1e44587a0318bea61c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027385"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="21981-103">Intune を使用して会社所有のデバイスを登録する</span><span class="sxs-lookup"><span data-stu-id="21981-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="21981-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="21981-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="21981-105">組織所有または会社所有のデバイスを登録して、デバイスの種類、デバイスの購入方法、組織のニーズに応じて、さまざまな方法で Intune で管理することができます。</span><span class="sxs-lookup"><span data-stu-id="21981-105">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="21981-106">また、ポータル サイト アプリをインストールして、会社所有のデバイスの登録と管理を、"Bring Your Own Device" (BYOD) のようなシナリオで行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="21981-106">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="21981-107">次の Graph リソースを使用して、Intune での会社所有のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="21981-107">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="21981-108">インポートした Windows AutoPilot デバイス ID</span><span class="sxs-lookup"><span data-stu-id="21981-108">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="21981-109">インポートした Windows AutoPilot デバイス ID のインポート状態</span><span class="sxs-lookup"><span data-stu-id="21981-109">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="21981-110">インポートした Windows AutoPilot デバイス ID の状態</span><span class="sxs-lookup"><span data-stu-id="21981-110">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="21981-111">インポートした Windows AutoPilot デバイス ID のアップロード</span><span class="sxs-lookup"><span data-stu-id="21981-111">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="21981-112">インポートした Windows AutoPilot デバイス ID のアップロードの状態</span><span class="sxs-lookup"><span data-stu-id="21981-112">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
