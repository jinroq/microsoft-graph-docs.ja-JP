---
title: deviceManagementExchangeConnector の作成
description: 新しい deviceManagementExchangeConnector オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 04794c97edef8495f2132cf556680678a5b63edf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348196"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="1a7be-103">deviceManagementExchangeConnector の作成</span><span class="sxs-lookup"><span data-stu-id="1a7be-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="1a7be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a7be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a7be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a7be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a7be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a7be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a7be-107">新しい [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1a7be-107">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a7be-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a7be-108">Prerequisites</span></span>
<span data-ttu-id="1a7be-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a7be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a7be-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a7be-111">Permission type</span></span>|<span data-ttu-id="1a7be-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a7be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a7be-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a7be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a7be-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a7be-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a7be-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a7be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a7be-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a7be-116">Not supported.</span></span>|
|<span data-ttu-id="1a7be-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a7be-117">Application</span></span>|<span data-ttu-id="1a7be-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a7be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a7be-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a7be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="1a7be-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a7be-120">Request headers</span></span>
|<span data-ttu-id="1a7be-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a7be-121">Header</span></span>|<span data-ttu-id="1a7be-122">値</span><span class="sxs-lookup"><span data-stu-id="1a7be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a7be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a7be-123">Authorization</span></span>|<span data-ttu-id="1a7be-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a7be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a7be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a7be-125">Accept</span></span>|<span data-ttu-id="1a7be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a7be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a7be-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a7be-127">Request body</span></span>
<span data-ttu-id="1a7be-128">要求本文で、deviceManagementExchangeConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a7be-128">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="1a7be-129">次の表に、deviceManagementExchangeConnector の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1a7be-129">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="1a7be-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a7be-130">Property</span></span>|<span data-ttu-id="1a7be-131">種類</span><span class="sxs-lookup"><span data-stu-id="1a7be-131">Type</span></span>|<span data-ttu-id="1a7be-132">説明</span><span class="sxs-lookup"><span data-stu-id="1a7be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a7be-133">ID</span><span class="sxs-lookup"><span data-stu-id="1a7be-133">id</span></span>|<span data-ttu-id="1a7be-134">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-134">String</span></span>|<span data-ttu-id="1a7be-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1a7be-135">Not yet documented</span></span>|
|<span data-ttu-id="1a7be-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1a7be-136">lastSyncDateTime</span></span>|<span data-ttu-id="1a7be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a7be-137">DateTimeOffset</span></span>|<span data-ttu-id="1a7be-138">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="1a7be-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="1a7be-139">status</span><span class="sxs-lookup"><span data-stu-id="1a7be-139">status</span></span>|[<span data-ttu-id="1a7be-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="1a7be-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="1a7be-141">Exchange コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="1a7be-141">Exchange Connector Status.</span></span> <span data-ttu-id="1a7be-142">可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="1a7be-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="1a7be-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1a7be-143">primarySmtpAddress</span></span>|<span data-ttu-id="1a7be-144">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-144">String</span></span>|<span data-ttu-id="1a7be-145">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="1a7be-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="1a7be-146">serverName</span><span class="sxs-lookup"><span data-stu-id="1a7be-146">serverName</span></span>|<span data-ttu-id="1a7be-147">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-147">String</span></span>|<span data-ttu-id="1a7be-148">Exchange サーバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="1a7be-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="1a7be-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="1a7be-149">connectorServerName</span></span>|<span data-ttu-id="1a7be-150">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-150">String</span></span>|<span data-ttu-id="1a7be-151">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="1a7be-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="1a7be-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="1a7be-152">exchangeConnectorType</span></span>|[<span data-ttu-id="1a7be-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="1a7be-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="1a7be-154">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="1a7be-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="1a7be-155">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="1a7be-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="1a7be-156">version</span><span class="sxs-lookup"><span data-stu-id="1a7be-156">version</span></span>|<span data-ttu-id="1a7be-157">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-157">String</span></span>|<span data-ttu-id="1a7be-158">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="1a7be-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="1a7be-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="1a7be-159">exchangeAlias</span></span>|<span data-ttu-id="1a7be-160">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-160">String</span></span>|<span data-ttu-id="1a7be-161">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="1a7be-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="1a7be-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="1a7be-162">exchangeOrganization</span></span>|<span data-ttu-id="1a7be-163">String</span><span class="sxs-lookup"><span data-stu-id="1a7be-163">String</span></span>|<span data-ttu-id="1a7be-164">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="1a7be-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="1a7be-165">応答</span><span class="sxs-lookup"><span data-stu-id="1a7be-165">Response</span></span>
<span data-ttu-id="1a7be-166">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1a7be-166">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a7be-167">例</span><span class="sxs-lookup"><span data-stu-id="1a7be-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a7be-168">要求</span><span class="sxs-lookup"><span data-stu-id="1a7be-168">Request</span></span>
<span data-ttu-id="1a7be-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a7be-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="1a7be-170">応答</span><span class="sxs-lookup"><span data-stu-id="1a7be-170">Response</span></span>
<span data-ttu-id="1a7be-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a7be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```





