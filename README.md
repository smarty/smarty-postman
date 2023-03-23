# Examples of the Smarty APIs using Postman Collections

-------------------------------------------- Under Development -------------------------------------------

Welcome to [Smarty](https://www.smarty.com), one of the fastest Address Verification and Geocoding services available! 

This repository exists to help you familiarize yourself with the different APIs that Smarty provides through the use of [Postman](https://www.postman.com). More specifically through a [Postman Collection](https://learning.postman.com/docs/collections/collections-overview/). 

This document will act as instructions for the collection, so we recommend opening the collection in a new tab or window.
Click the button below to get started. Once a popup appears asking if you'd like to fork the repository, press the button that says fork.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/26425577-872d9849-4309-44b4-8be5-5a33cd0abdc1?action=collection%2Ffork&collection-url=entityId%3D26425577-872d9849-4309-44b4-8be5-5a33cd0abdc1%26entityType%3Dcollection%26workspaceId%3D04903370-4703-4fcc-83d9-ccfe557f9e37#?env%5BSmarty%20-%20Live%20Deployment%5D=W3sia2V5IjoiYXV0aC1pZCIsInZhbHVlIjoiWU9VUl9BVVRIX19JRCIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJzZWNyZXQiLCJzZXNzaW9uVmFsdWUiOiJiOGNkNzg1Mi00MTlmLTg0MjYtNWNmOC0wYjA0ZDExMDA1ZmMiLCJzZXNzaW9uSW5kZXgiOjB9LHsia2V5IjoiYXV0aC10b2tlbiIsInZhbHVlIjoiWU9VUl9BVVRIX1RPS0VOIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6InNlY3JldCIsInNlc3Npb25WYWx1ZSI6ImQ5TWw3bXBvS1M3Z0VmN2pxRjhhIiwic2Vzc2lvbkluZGV4IjoxfSx7ImtleSI6ImxpY2Vuc2UiLCJ2YWx1ZSI6IllPVVJfTElDRU5TRSIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoidXMtY29yZS1jbG91ZCIsInNlc3Npb25JbmRleCI6Mn0seyJrZXkiOiJ1cmwiLCJ2YWx1ZSI6ImFwaS5zbWFydHkuY29tIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiJhcGkuc21hcnR5LmNvbSIsInNlc3Npb25JbmRleCI6M30seyJrZXkiOiJpbnB1dF9pZCIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjR9LHsia2V5Ijoic3RyZWV0IiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6NX0seyJrZXkiOiJzdHJlZXQyIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6Nn0seyJrZXkiOiJzZWNvbmRhcnkiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4Ijo3fSx7ImtleSI6ImNpdHkiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4Ijo4fSx7ImtleSI6InN0YXRlIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6OX0seyJrZXkiOiJ6aXBjb2RlIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6MTB9LHsia2V5IjoibGFzdGxpbmUiLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4IjoxMX0seyJrZXkiOiJhZHJlc3NlZSIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjEyfSx7ImtleSI6InVyYmFuaXphdGlvbiIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjEzfSx7ImtleSI6ImNhbmRpZGF0ZXMiLCJ2YWx1ZSI6IjEwIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIxMCIsInNlc3Npb25JbmRleCI6MTR9LHsia2V5IjoibWF0Y2giLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4IjoxNX1d)


