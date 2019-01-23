---
title: DeviceConfigurationConflictSummary を作成します。
description: 新しい deviceConfigurationConflictSummary オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9488f61819a67f7ab648a6677a30e7422be0539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412080"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="63749-103">DeviceConfigurationConflictSummary を作成します。</span><span class="sxs-lookup"><span data-stu-id="63749-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="63749-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63749-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63749-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63749-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63749-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63749-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63749-107">新しい[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="63749-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63749-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="63749-108">Prerequisites</span></span>
<span data-ttu-id="63749-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63749-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63749-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63749-111">Permission type</span></span>|<span data-ttu-id="63749-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="63749-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63749-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63749-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63749-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63749-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63749-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63749-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63749-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63749-116">Not supported.</span></span>|
|<span data-ttu-id="63749-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63749-117">Application</span></span>|<span data-ttu-id="63749-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63749-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63749-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63749-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="63749-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63749-120">Request headers</span></span>
|<span data-ttu-id="63749-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63749-121">Header</span></span>|<span data-ttu-id="63749-122">値</span><span class="sxs-lookup"><span data-stu-id="63749-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63749-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63749-123">Authorization</span></span>|<span data-ttu-id="63749-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="63749-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63749-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63749-125">Accept</span></span>|<span data-ttu-id="63749-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63749-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63749-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="63749-127">Request body</span></span>
<span data-ttu-id="63749-128">要求の本文に deviceConfigurationConflictSummary オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="63749-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="63749-129">次の表は、deviceConfigurationConflictSummary を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="63749-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="63749-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63749-130">Property</span></span>|<span data-ttu-id="63749-131">型</span><span class="sxs-lookup"><span data-stu-id="63749-131">Type</span></span>|<span data-ttu-id="63749-132">説明</span><span class="sxs-lookup"><span data-stu-id="63749-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63749-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="63749-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="63749-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="63749-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="63749-135">一連のポリシーを指定された設定と競合していません。</span><span class="sxs-lookup"><span data-stu-id="63749-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="63749-136">id</span><span class="sxs-lookup"><span data-stu-id="63749-136">id</span></span>|<span data-ttu-id="63749-137">String</span><span class="sxs-lookup"><span data-stu-id="63749-137">String</span></span>|<span data-ttu-id="63749-138">競合するポリシーのセットの id です。</span><span class="sxs-lookup"><span data-stu-id="63749-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="63749-139">この id では、ConflictingDeviceConfigurations 内のすべてのポリシーの id をアンダー スコアで区切られた辞書式の順序にします。</span><span class="sxs-lookup"><span data-stu-id="63749-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="63749-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="63749-140">contributingSettings</span></span>|<span data-ttu-id="63749-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="63749-141">String collection</span></span>|<span data-ttu-id="63749-142">一連の特定のポリシーと競合の設定</span><span class="sxs-lookup"><span data-stu-id="63749-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="63749-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="63749-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="63749-144">Int32</span><span class="sxs-lookup"><span data-stu-id="63749-144">Int32</span></span>|<span data-ttu-id="63749-145">チェックインの競合しているポリシーと設定の影響を受ける数</span><span class="sxs-lookup"><span data-stu-id="63749-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="63749-146">応答</span><span class="sxs-lookup"><span data-stu-id="63749-146">Response</span></span>
<span data-ttu-id="63749-147">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="63749-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63749-148">例</span><span class="sxs-lookup"><span data-stu-id="63749-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="63749-149">要求</span><span class="sxs-lookup"><span data-stu-id="63749-149">Request</span></span>
<span data-ttu-id="63749-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="63749-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="63749-151">応答</span><span class="sxs-lookup"><span data-stu-id="63749-151">Response</span></span>
<span data-ttu-id="63749-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="63749-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




