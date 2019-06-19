---
title: DeviceManagementDomainJoinConnector の更新
description: DeviceManagementDomainJoinConnector オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 760683b2b837ac8bcfab40a12b3bf4f84214d2c2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002155"
---
# <a name="update-devicemanagementdomainjoinconnector"></a><span data-ttu-id="28f1f-103">DeviceManagementDomainJoinConnector の更新</span><span class="sxs-lookup"><span data-stu-id="28f1f-103">Update deviceManagementDomainJoinConnector</span></span>

> <span data-ttu-id="28f1f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28f1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28f1f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28f1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28f1f-106">[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="28f1f-106">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28f1f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="28f1f-107">Prerequisites</span></span>
<span data-ttu-id="28f1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28f1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28f1f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28f1f-110">Permission type</span></span>|<span data-ttu-id="28f1f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="28f1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28f1f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28f1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28f1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28f1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28f1f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28f1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28f1f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28f1f-115">Not supported.</span></span>|
|<span data-ttu-id="28f1f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28f1f-116">Application</span></span>|<span data-ttu-id="28f1f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28f1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28f1f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28f1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="28f1f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28f1f-119">Request headers</span></span>
|<span data-ttu-id="28f1f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28f1f-120">Header</span></span>|<span data-ttu-id="28f1f-121">値</span><span class="sxs-lookup"><span data-stu-id="28f1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28f1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28f1f-122">Authorization</span></span>|<span data-ttu-id="28f1f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="28f1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28f1f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="28f1f-124">Accept</span></span>|<span data-ttu-id="28f1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28f1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28f1f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="28f1f-126">Request body</span></span>
<span data-ttu-id="28f1f-127">要求本文で、 [Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="28f1f-127">In the request body, supply a JSON representation for the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>

<span data-ttu-id="28f1f-128">次の表に、 [Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="28f1f-128">The following table shows the properties that are required when you create the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>

|<span data-ttu-id="28f1f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f1f-129">Property</span></span>|<span data-ttu-id="28f1f-130">型</span><span class="sxs-lookup"><span data-stu-id="28f1f-130">Type</span></span>|<span data-ttu-id="28f1f-131">説明</span><span class="sxs-lookup"><span data-stu-id="28f1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28f1f-132">id</span><span class="sxs-lookup"><span data-stu-id="28f1f-132">id</span></span>|<span data-ttu-id="28f1f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="28f1f-133">String</span></span>|<span data-ttu-id="28f1f-134">コネクタを表す一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="28f1f-134">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="28f1f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="28f1f-135">displayName</span></span>|<span data-ttu-id="28f1f-136">String</span><span class="sxs-lookup"><span data-stu-id="28f1f-136">String</span></span>|<span data-ttu-id="28f1f-137">コネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="28f1f-137">The connector display name.</span></span>|
|<span data-ttu-id="28f1f-138">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="28f1f-138">lastConnectionDateTime</span></span>|<span data-ttu-id="28f1f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28f1f-139">DateTimeOffset</span></span>|<span data-ttu-id="28f1f-140">前回のコネクタが Intune に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="28f1f-140">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="28f1f-141">state</span><span class="sxs-lookup"><span data-stu-id="28f1f-141">state</span></span>|[<span data-ttu-id="28f1f-142">Devicemanagementdomainjoinコネクタ状態</span><span class="sxs-lookup"><span data-stu-id="28f1f-142">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="28f1f-143">コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="28f1f-143">The connector state.</span></span> <span data-ttu-id="28f1f-144">可能な値は、`active`、`error`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="28f1f-144">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="28f1f-145">version</span><span class="sxs-lookup"><span data-stu-id="28f1f-145">version</span></span>|<span data-ttu-id="28f1f-146">String</span><span class="sxs-lookup"><span data-stu-id="28f1f-146">String</span></span>|<span data-ttu-id="28f1f-147">コネクタのバージョン。</span><span class="sxs-lookup"><span data-stu-id="28f1f-147">The version of the connector.</span></span>|



## <a name="response"></a><span data-ttu-id="28f1f-148">応答</span><span class="sxs-lookup"><span data-stu-id="28f1f-148">Response</span></span>
<span data-ttu-id="28f1f-149">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementdomainjoinconnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28f1f-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28f1f-150">例</span><span class="sxs-lookup"><span data-stu-id="28f1f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="28f1f-151">要求</span><span class="sxs-lookup"><span data-stu-id="28f1f-151">Request</span></span>
<span data-ttu-id="28f1f-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28f1f-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/domainJoinConnectors/{deviceManagementDomainJoinConnectorId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="28f1f-153">応答</span><span class="sxs-lookup"><span data-stu-id="28f1f-153">Response</span></span>
<span data-ttu-id="28f1f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28f1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "77296cf7-6cf7-7729-f76c-2977f76c2977",
  "displayName": "Display Name value",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "error",
  "version": "Version value"
}
```




