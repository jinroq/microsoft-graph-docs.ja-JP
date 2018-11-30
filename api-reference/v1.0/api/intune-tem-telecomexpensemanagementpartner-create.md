---
title: telecomExpenseManagementPartner の作成
description: 新しい telecomExpenseManagementPartner オブジェクトを作成します。
ms.openlocfilehash: 327c2be4f84ea16d56a068db10c87e9d776b89c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022807"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="eed95-103">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="eed95-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="eed95-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eed95-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eed95-105">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eed95-105">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eed95-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="eed95-106">Prerequisites</span></span>
<span data-ttu-id="eed95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eed95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed95-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eed95-109">Permission type</span></span>|<span data-ttu-id="eed95-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eed95-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eed95-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eed95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eed95-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eed95-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eed95-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eed95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eed95-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eed95-114">Not supported.</span></span>|
|<span data-ttu-id="eed95-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eed95-115">Application</span></span>|<span data-ttu-id="eed95-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eed95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eed95-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eed95-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="eed95-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eed95-118">Request headers</span></span>
|<span data-ttu-id="eed95-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eed95-119">Header</span></span>|<span data-ttu-id="eed95-120">値</span><span class="sxs-lookup"><span data-stu-id="eed95-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eed95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eed95-121">Authorization</span></span>|<span data-ttu-id="eed95-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="eed95-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eed95-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eed95-123">Accept</span></span>|<span data-ttu-id="eed95-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eed95-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eed95-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eed95-125">Request body</span></span>
<span data-ttu-id="eed95-126">要求本文で、telecomExpenseManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eed95-126">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="eed95-127">次の表に、telecomExpenseManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eed95-127">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="eed95-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eed95-128">Property</span></span>|<span data-ttu-id="eed95-129">型</span><span class="sxs-lookup"><span data-stu-id="eed95-129">Type</span></span>|<span data-ttu-id="eed95-130">説明</span><span class="sxs-lookup"><span data-stu-id="eed95-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eed95-131">id</span><span class="sxs-lookup"><span data-stu-id="eed95-131">id</span></span>|<span data-ttu-id="eed95-132">String</span><span class="sxs-lookup"><span data-stu-id="eed95-132">String</span></span>|<span data-ttu-id="eed95-133">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="eed95-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="eed95-134">displayName</span><span class="sxs-lookup"><span data-stu-id="eed95-134">displayName</span></span>|<span data-ttu-id="eed95-135">String</span><span class="sxs-lookup"><span data-stu-id="eed95-135">String</span></span>|<span data-ttu-id="eed95-136">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="eed95-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="eed95-137">url</span><span class="sxs-lookup"><span data-stu-id="eed95-137">url</span></span>|<span data-ttu-id="eed95-138">String</span><span class="sxs-lookup"><span data-stu-id="eed95-138">String</span></span>|<span data-ttu-id="eed95-139">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="eed95-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="eed95-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="eed95-140">appAuthorized</span></span>|<span data-ttu-id="eed95-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="eed95-141">Boolean</span></span>|<span data-ttu-id="eed95-142">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="eed95-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="eed95-143">enabled</span><span class="sxs-lookup"><span data-stu-id="eed95-143">enabled</span></span>|<span data-ttu-id="eed95-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="eed95-144">Boolean</span></span>|<span data-ttu-id="eed95-145">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="eed95-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="eed95-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="eed95-146">lastConnectionDateTime</span></span>|<span data-ttu-id="eed95-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eed95-147">DateTimeOffset</span></span>|<span data-ttu-id="eed95-148">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="eed95-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="eed95-149">応答</span><span class="sxs-lookup"><span data-stu-id="eed95-149">Response</span></span>
<span data-ttu-id="eed95-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eed95-150">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eed95-151">例</span><span class="sxs-lookup"><span data-stu-id="eed95-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="eed95-152">要求</span><span class="sxs-lookup"><span data-stu-id="eed95-152">Request</span></span>
<span data-ttu-id="eed95-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eed95-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="eed95-154">応答</span><span class="sxs-lookup"><span data-stu-id="eed95-154">Response</span></span>
<span data-ttu-id="eed95-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eed95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



