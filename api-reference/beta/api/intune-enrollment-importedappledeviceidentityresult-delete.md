---
title: ImportedAppleDeviceIdentityResult を削除します。
description: ImportedAppleDeviceIdentityResult を削除します。
author: tfitzmac
ms.openlocfilehash: 0a9be53ea8fa0084ae235417d757cc0a85a4120e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359998"
---
# <a name="delete-importedappledeviceidentityresult"></a><span data-ttu-id="fa089-103">ImportedAppleDeviceIdentityResult を削除します。</span><span class="sxs-lookup"><span data-stu-id="fa089-103">Delete importedAppleDeviceIdentityResult</span></span>

> <span data-ttu-id="fa089-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa089-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa089-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa089-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa089-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa089-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa089-107">の[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="fa089-107">Deletes a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa089-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa089-108">Prerequisites</span></span>
<span data-ttu-id="fa089-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa089-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa089-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa089-111">Permission type</span></span>|<span data-ttu-id="fa089-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa089-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa089-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa089-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa089-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa089-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa089-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa089-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa089-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa089-116">Not supported.</span></span>|
|<span data-ttu-id="fa089-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa089-117">Application</span></span>|<span data-ttu-id="fa089-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa089-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa089-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa089-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="fa089-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa089-120">Request headers</span></span>
|<span data-ttu-id="fa089-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa089-121">Header</span></span>|<span data-ttu-id="fa089-122">値</span><span class="sxs-lookup"><span data-stu-id="fa089-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa089-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa089-123">Authorization</span></span>|<span data-ttu-id="fa089-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fa089-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa089-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa089-125">Accept</span></span>|<span data-ttu-id="fa089-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa089-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa089-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa089-127">Request body</span></span>
<span data-ttu-id="fa089-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa089-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa089-129">応答</span><span class="sxs-lookup"><span data-stu-id="fa089-129">Response</span></span>
<span data-ttu-id="fa089-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fa089-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fa089-131">例</span><span class="sxs-lookup"><span data-stu-id="fa089-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa089-132">要求</span><span class="sxs-lookup"><span data-stu-id="fa089-132">Request</span></span>
<span data-ttu-id="fa089-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa089-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="fa089-134">応答</span><span class="sxs-lookup"><span data-stu-id="fa089-134">Response</span></span>
<span data-ttu-id="fa089-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa089-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





