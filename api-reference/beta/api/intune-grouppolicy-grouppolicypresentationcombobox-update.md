---
title: GroupPolicyPresentationComboBox を更新します。
description: GroupPolicyPresentationComboBox オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6302d52e91e5fe1cf8a21e525d0eccef608b3b24
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430465"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="b794f-103">GroupPolicyPresentationComboBox を更新します。</span><span class="sxs-lookup"><span data-stu-id="b794f-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="b794f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b794f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b794f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b794f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b794f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b794f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b794f-107">[GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b794f-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b794f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b794f-108">Prerequisites</span></span>
<span data-ttu-id="b794f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b794f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b794f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b794f-111">Permission type</span></span>|<span data-ttu-id="b794f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b794f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b794f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b794f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b794f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b794f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b794f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b794f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b794f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b794f-116">Not supported.</span></span>|
|<span data-ttu-id="b794f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b794f-117">Application</span></span>|<span data-ttu-id="b794f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b794f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b794f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b794f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="b794f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b794f-120">Request headers</span></span>
|<span data-ttu-id="b794f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b794f-121">Header</span></span>|<span data-ttu-id="b794f-122">値</span><span class="sxs-lookup"><span data-stu-id="b794f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b794f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b794f-123">Authorization</span></span>|<span data-ttu-id="b794f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b794f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b794f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b794f-125">Accept</span></span>|<span data-ttu-id="b794f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b794f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b794f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b794f-127">Request body</span></span>
<span data-ttu-id="b794f-128">要求の本文に[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b794f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="b794f-129">[GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b794f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="b794f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b794f-130">Property</span></span>|<span data-ttu-id="b794f-131">型</span><span class="sxs-lookup"><span data-stu-id="b794f-131">Type</span></span>|<span data-ttu-id="b794f-132">説明</span><span class="sxs-lookup"><span data-stu-id="b794f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b794f-133">label</span><span class="sxs-lookup"><span data-stu-id="b794f-133">label</span></span>|<span data-ttu-id="b794f-134">String</span><span class="sxs-lookup"><span data-stu-id="b794f-134">String</span></span>|<span data-ttu-id="b794f-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="b794f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b794f-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="b794f-136">The default value is empty.</span></span> <span data-ttu-id="b794f-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b794f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b794f-138">id</span><span class="sxs-lookup"><span data-stu-id="b794f-138">id</span></span>|<span data-ttu-id="b794f-139">String</span><span class="sxs-lookup"><span data-stu-id="b794f-139">String</span></span>|<span data-ttu-id="b794f-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b794f-140">Key of the entity.</span></span> <span data-ttu-id="b794f-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b794f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b794f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b794f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b794f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b794f-143">DateTimeOffset</span></span>|<span data-ttu-id="b794f-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="b794f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="b794f-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="b794f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b794f-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b794f-146">defaultValue</span></span>|<span data-ttu-id="b794f-147">文字列</span><span class="sxs-lookup"><span data-stu-id="b794f-147">String</span></span>|<span data-ttu-id="b794f-148">コンボ ボックスに表示される既定の文字列をローカライズします。</span><span class="sxs-lookup"><span data-stu-id="b794f-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="b794f-149">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="b794f-149">The default value is empty.</span></span>|
|<span data-ttu-id="b794f-150">提案</span><span class="sxs-lookup"><span data-stu-id="b794f-150">suggestions</span></span>|<span data-ttu-id="b794f-151">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b794f-151">String collection</span></span>|<span data-ttu-id="b794f-152">ローカライズされた文字列がコンボ ボックスのドロップダウン リストに一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b794f-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="b794f-153">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="b794f-153">The default value is empty.</span></span>|
|<span data-ttu-id="b794f-154">必須</span><span class="sxs-lookup"><span data-stu-id="b794f-154">required</span></span>|<span data-ttu-id="b794f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="b794f-155">Boolean</span></span>|<span data-ttu-id="b794f-156">パラメーターの値を指定する必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b794f-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="b794f-157">既定値は、false を指定します。</span><span class="sxs-lookup"><span data-stu-id="b794f-157">The default value is false.</span></span>|
|<span data-ttu-id="b794f-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="b794f-158">maxLength</span></span>|<span data-ttu-id="b794f-159">Int64</span><span class="sxs-lookup"><span data-stu-id="b794f-159">Int64</span></span>|<span data-ttu-id="b794f-160">パラメーターのテキスト文字の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="b794f-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="b794f-161">既定値は、1023 です。</span><span class="sxs-lookup"><span data-stu-id="b794f-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="b794f-162">応答</span><span class="sxs-lookup"><span data-stu-id="b794f-162">Response</span></span>
<span data-ttu-id="b794f-163">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b794f-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b794f-164">例</span><span class="sxs-lookup"><span data-stu-id="b794f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b794f-165">要求</span><span class="sxs-lookup"><span data-stu-id="b794f-165">Request</span></span>
<span data-ttu-id="b794f-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b794f-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="b794f-167">応答</span><span class="sxs-lookup"><span data-stu-id="b794f-167">Response</span></span>
<span data-ttu-id="b794f-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b794f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```




