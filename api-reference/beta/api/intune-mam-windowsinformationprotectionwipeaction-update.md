---
title: WindowsInformationProtectionWipeAction を更新します。
description: WindowsInformationProtectionWipeAction オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49b79d6ebd12d81332613c646623d68dc0b09a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430414"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="76db8-103">WindowsInformationProtectionWipeAction を更新します。</span><span class="sxs-lookup"><span data-stu-id="76db8-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="76db8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76db8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76db8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76db8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76db8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76db8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76db8-107">[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="76db8-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76db8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="76db8-108">Prerequisites</span></span>
<span data-ttu-id="76db8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76db8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="76db8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76db8-111">Permission type</span></span>|<span data-ttu-id="76db8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76db8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76db8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76db8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76db8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76db8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76db8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76db8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76db8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76db8-116">Not supported.</span></span>|
|<span data-ttu-id="76db8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76db8-117">Application</span></span>|<span data-ttu-id="76db8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76db8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76db8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76db8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="76db8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76db8-120">Request headers</span></span>
|<span data-ttu-id="76db8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76db8-121">Header</span></span>|<span data-ttu-id="76db8-122">値</span><span class="sxs-lookup"><span data-stu-id="76db8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76db8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76db8-123">Authorization</span></span>|<span data-ttu-id="76db8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="76db8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76db8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76db8-125">Accept</span></span>|<span data-ttu-id="76db8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76db8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76db8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="76db8-127">Request body</span></span>
<span data-ttu-id="76db8-128">要求の本文に[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="76db8-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="76db8-129">[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="76db8-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="76db8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76db8-130">Property</span></span>|<span data-ttu-id="76db8-131">型</span><span class="sxs-lookup"><span data-stu-id="76db8-131">Type</span></span>|<span data-ttu-id="76db8-132">説明</span><span class="sxs-lookup"><span data-stu-id="76db8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76db8-133">id</span><span class="sxs-lookup"><span data-stu-id="76db8-133">id</span></span>|<span data-ttu-id="76db8-134">String</span><span class="sxs-lookup"><span data-stu-id="76db8-134">String</span></span>|<span data-ttu-id="76db8-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="76db8-135">Key of the entity.</span></span>|
|<span data-ttu-id="76db8-136">status</span><span class="sxs-lookup"><span data-stu-id="76db8-136">status</span></span>|[<span data-ttu-id="76db8-137">actionState</span><span class="sxs-lookup"><span data-stu-id="76db8-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="76db8-138">アクションのステータスを消去します。</span><span class="sxs-lookup"><span data-stu-id="76db8-138">Wipe action status.</span></span> <span data-ttu-id="76db8-139">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="76db8-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="76db8-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="76db8-140">targetedUserId</span></span>|<span data-ttu-id="76db8-141">String</span><span class="sxs-lookup"><span data-stu-id="76db8-141">String</span></span>|<span data-ttu-id="76db8-142">このワイプ操作のターゲットとなるユーザーの Id。</span><span class="sxs-lookup"><span data-stu-id="76db8-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="76db8-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="76db8-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="76db8-144">String</span><span class="sxs-lookup"><span data-stu-id="76db8-144">String</span></span>|<span data-ttu-id="76db8-145">このワイプ操作のターゲットとなる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="76db8-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="76db8-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="76db8-146">targetedDeviceName</span></span>|<span data-ttu-id="76db8-147">String</span><span class="sxs-lookup"><span data-stu-id="76db8-147">String</span></span>|<span data-ttu-id="76db8-148">ターゲット ・ デバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="76db8-148">Targeted device name.</span></span>|
|<span data-ttu-id="76db8-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="76db8-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="76db8-150">String</span><span class="sxs-lookup"><span data-stu-id="76db8-150">String</span></span>|<span data-ttu-id="76db8-151">ターゲット デバイスの Mac アドレスです。</span><span class="sxs-lookup"><span data-stu-id="76db8-151">Targeted device Mac address.</span></span>|



## <a name="response"></a><span data-ttu-id="76db8-152">応答</span><span class="sxs-lookup"><span data-stu-id="76db8-152">Response</span></span>
<span data-ttu-id="76db8-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="76db8-153">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76db8-154">例</span><span class="sxs-lookup"><span data-stu-id="76db8-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="76db8-155">要求</span><span class="sxs-lookup"><span data-stu-id="76db8-155">Request</span></span>
<span data-ttu-id="76db8-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76db8-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```

### <a name="response"></a><span data-ttu-id="76db8-157">応答</span><span class="sxs-lookup"><span data-stu-id="76db8-157">Response</span></span>
<span data-ttu-id="76db8-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76db8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```




