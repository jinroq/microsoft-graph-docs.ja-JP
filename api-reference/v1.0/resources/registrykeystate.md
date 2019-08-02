---
title: registryKeyState リソースの種類
description: 通知に関連するレジストリキーの変更に関する情報、およびレジストリキーを変更したプロセスについて説明します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2c68206dc61603324fe346a57da81129b4fe5425
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034798"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState リソースの種類

通知に関連するレジストリキーの変更に関する情報、およびレジストリキーを変更したプロセスについて説明します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|レジストリ|registryHive|[Windows レジストリハイブ](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives): <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\限り.</li></ul> 可能な値は、`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault` です。|
|キー|String|Current (つまり変更された) レジストリキー (ハイブを除外)。|
|oldKey|String|Previous (変更前) レジストリキー (ハイブを除外)。|
|oldValueData|String|以前の (変更前) レジストリキー値のデータ (内容)。|
|oldValueName|String|Previous (変更前) レジストリキー値の名前。|
|operation|registryOperation|レジストリキー名と値の一方または両方を変更した操作。 使用可能な値は、`unknown`、`create`、`modify`、`delete` です。|
|processId|Int32|レジストリキーを変更したプロセスのプロセス ID (PID) (プロセスの詳細は、警告の「プロセス」のコレクションに表示されます)。|
|valueData|String|現在の (つまり変更された) レジストリキー値のデータ (内容)。|
|valueName|String|Current (変更された) レジストリキー値の名前|
|valueType|registryValueType|[レジストリキーの値の種類](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> 可能な値は、`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
